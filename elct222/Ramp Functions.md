### In Octave

```Matlab
function f = ramp(t)
	f = (sign(t) + 1) * 0.5;
	f = f .* t;
end
```

### Uses
- Trapezoidal Pulse
	- Uses 4 ramp functions in the following order: +, -, -, +
- Triangle Pulse
	- Uses 3 ramp functions in the following order: +, 2-, +
		- Second ramp function is double the magnitude of the other two
	

