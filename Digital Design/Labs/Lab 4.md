Branch type:
```Systemverilog
assign branch_offset_EX = 
	{instr_EX[31], instr_EX[7], instr_EX[30:25], instr_EX11:8]}

assign branch_addr_EX = PC_EX + {branch_offset_EX} ...
```

J type:
```Systemverilog
assign jal_offset_EX = {instr_EX[31], instr_EX[19:12], instr_EX[20], instr_EX[30:21], 1'b0};
assign jal_addr_EX = PC_EX + jal_offset_EX[13:2];
```

| Branch FETCH | Branch EX / Fall-through Fetch            | Branch WB / Target Fetch               |
| ------------ | ----------------------------------------- | -------------------------------------- |
| Increment PC | Use the result of the ALU to change pcsrc | Use pcsrc to determine val of PC_FETCH |
|              | Do calculations for B-type                |                                        |
|              | Initiate a NOOP in CU                     |                                        |
|              | Use pcsrc to get next pcfetch                                          |                                        |


| Misc                                   | FETCH                        | EX  | WB  |
| -------------------------------------- | ---------------------------- | --- | --- |
| Figure out next instruction's PC value | Change current PC to next PC |     |     |


If stall_FETCH
- Keep PC_FETCH
- instr_EX <= 32'b0
- NO REG WRITES


### Branch that isn't taken
| Instruction        |     |     |     |     |     |     |
| ------------------ | --- | --- | --- | --- | --- | --- |
| add                | F   | E   | W   |     |     |     |
| branch (not taken) |     | F   | E   | W   |     |     |
| stall              |     |     | F   | E   | W   |     |
| add                |     |     |     | F   | E   | W   |
- PC at the last add will be 1 less than if it had been incremented normally

### Branch that is taken
| Instruction |     |     |     |     |     |     |
| ----------- | --- | --- | --- | --- | --- | --- |
| add         | F   | E   | W   |     |     |     |
| branch      |     | F   | E   | W   |     |     |
| stall       |     |     | F   | E   | W   |     |
| target      |     |     |     | F   | E   | W   |


### PC status
|               | Stall      | Not Stall           |
| ------------- | ---------- | ------------------- |
| pcsrc = 00    | keep       | PC_Fetch ++         |
| anything else | go to addr | Should never happen |

- Use display to test that that there is never a case where not stall and pcsrc != 00 happens

```SystemVerilog
// In CU
// Remove the first if statement for stall and add
if (stall_EX) begin
	gpio_we = 1'b0
	regwrite = 1'b0
end

```
also make sure to add regsel and regwrite to jal and jalr

| Inst   |     |     |     |     |     |     |
| ------ | --- | --- | --- | --- | --- | --- |
| add    | F   | E   | W   |     |     |     |
| branch |     | F   | E   | W   |     |     |
| stall  |     |     | F   | E   | W   |     |
| branch |     |     |     | F   | E   | W   | 
