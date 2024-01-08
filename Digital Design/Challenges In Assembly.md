1. Make sure you load words into registers before operations
2. Always complement branch logic before use
3. 

##### Summation Example

```asm
.text
main:
	li a7, 5
	ecall

	# Initializing the index and sum variables
	addi t0, x0. 0
	addi s0, x0, 0
sum_loop:
	bge s0, a0, print
	addi t0, t0, 1
	add s0, s0, t0
	
	j sum_loop
print:
	mv a0, t0
	li a7, 1
	ecall
exit:
	li a7, 10
	ecall
```

- a7 acts as params for ecall (syscall)

##### 32 bit Float Example 
```asm
.data
	const: .word 0x0000000B
.text
main:
	li a7, 5
	ecall

	slli a0, a0, 14
	
	# Setting up the constant 2.75 in (32,14) fixed point representation
	la t0, const
	lw t1. 0(t0)
	slli t1, 12
	
	# Initializing the index and sum variables
	addi t0, x0. 0
	addi s0, x0, 0
sum_loop:
	bge s0, a0, print
	addi t0, t0, 1

	# recast the index number in (32,14) fixed-point representation
	slli t2, t0, 14
	# add t2<-t2+2.75
	add s0, s0, t0
	
	mul t3, t2, t2
	mulh t4, t2,t2
	# Converting two seperate registers back into (32,14)
	srli t3, t3, 18
	slli t4, t4, 18
	or t5, t4, t3

	j sum_loop
print:
	mv a0, t0
	li a7, 1
	ecall
exit:
	li a7, 10
	ecall
```

```python
print("f")

```