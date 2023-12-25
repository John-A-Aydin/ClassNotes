Instead of
```SystemVerilog
assign {a,b} = c & d
```
we can use
```SystemVerilog
always_comb
	begin
		a = c
		b = d
	end
```
Always statements have a implied sensitivity list when they use \_comb
This tells us that the always statement is using [[Combinational Logic]]


##### always_ff
```SystemVerilog
always_ff @(sensitivity list, eg postedge clk)
	statement
```
In always_ff we need to use <= instead of =

##### D-Flip-Flop using always_ff
```SystemVerilog
module flopr(input clk,
			 input reset,
			input [3:0] d,
			output logic [3:0] q);
	// synchronous reset 
	always_ff @(posedge clk)
		if (reset) q <= 4'b0;
		else       q <= d;
endmodule
```