
```SystemVerilog
logic [31:0] mem[8191:0];
logic [12:0] addr;
logic [31:0] readdata, writedata;
logic we, clk;

initial $readmemh("mem.txt", mem);

assign readdata = mem[addr];
always_ff @(postedge clk)
	if (we) mem[addr] <= writedata;

```

One write per clock cycle, but as many reads as we want