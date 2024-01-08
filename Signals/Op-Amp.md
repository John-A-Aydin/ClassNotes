##### Operational Amplifier
- Two input terminals
	- positive (non inverting)
	- negative (inverting)
- One output
- Power +Vcc and -Vcc

![[Op-amp-diagram.png]]


### Ideal Op-Amp

Voltage and Current constraint
$$\Large v_p = v_n = 0$$$$\Large i_p=i_n=0$$


### Gain
- Open loop gain (A)$$\Large V_0 = A(V_p-V_n)$$
	- Linear response
- Closed loop gain (G)

### Operations

##### Integrators

	![[Op-Amp-integrator.png]]
$$\Large{v_{out}(t) = -\frac{1}{RC}\int^{t}_{t_0}{v_i dt+v_{out}(t_0)}}$$
##### Differentiator
![[Op-Amp-differentiator.png]]
$$\Large{v_{out} = - RC\frac{dv_i}{dt}}$$
