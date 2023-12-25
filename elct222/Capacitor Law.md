The voltage across a capacitor cannot instantly change.
#### $$\Large i=C\frac{dv}{dt} $$
or
#### $$\Large v(t) = \frac{1}C \int_{t_0}^t idt+v(t_0) $$
Capacitor law tells us that the current is proportional to the [[Capacitance]] and derivative of the voltage over time.

#### [[Energy]] Stored in Capacitor

#### $$\large w = \frac{1}2 Cv^2 $$

![[properties-capacitance-inductance.png]]

#### [[DC]]
- Capacitors act as an open circuit or unconnected wire in DC


### RC Circuits Charging$$V(t)=V_0(1-e^{-\frac{t}{\tau}})$$$$V(t)=V_{inf}+\Big[V_0-V_{inf})\Big]e^{-t/\tau}$$
##### In Octave:
```MatLab
C=<val>;
R=<val>;
t=<val>;
V=<val>;
tau=R/C;

V1t = V1inf + (V10 - V1inf)*exp(-t/tau);
# or
Vlt = V1(1 - exp(-t/tau));
```

### RC Circuits Discharging$$V(t)=V_0e^{-t/\tau}$$
