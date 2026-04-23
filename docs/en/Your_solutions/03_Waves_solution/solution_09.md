Here is the breakdown of the damped harmonic oscillator, followed by an interactive simulation where you can investigate the effects of the damping parameter using numerical integration (Runge-Kutta 4th order).

### **1. The General Solution**
The differential equation for a damped harmonic oscillator is:
$$m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0$$

To solve this linear, second-order, homogeneous differential equation, we assume a solution of the form $x(t) = e^{rt}$. Substituting this into the equation yields the **characteristic equation**:
$$mr^2 + br + k = 0$$

Using the quadratic formula, we find the roots of this equation:
$$r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}$$

The nature of these roots—and therefore the physical behavior of the system—depends entirely on the quantity under the square root, $b^2 - 4mk$. 

### **2. Classification of Damping Cases**
We classify the behavior of the oscillator into three distinct regimes based on the value of the damping parameter $b$ compared to the critical damping threshold, $b_c = 2\sqrt{mk}$.

**Case 1: Underdamped ($b^2 - 4mk < 0$, or $b < 2\sqrt{mk}$)**
* **Mathematical Result:** The roots $r_1$ and $r_2$ are complex conjugates.
* **General Solution:** $$x(t) = e^{-\frac{b}{2m}t} \left( C_1 \cos(\omega_d t) + C_2 \sin(\omega_d t) \right)$$ 
    where the damped angular frequency is $\omega_d = \frac{\sqrt{4mk - b^2}}{2m}$.
* **Physical Behavior:** The system oscillates, crossing the equilibrium point multiple times, but the amplitude exponentially decays over time due to friction/damping.

**Case 2: Critically Damped ($b^2 - 4mk = 0$, or $b = 2\sqrt{mk}$)**
* **Mathematical Result:** The roots are real and repeated ($r_1 = r_2 = -\frac{b}{2m}$).
* **General Solution:** $$x(t) = (C_1 + C_2 t) e^{-\frac{b}{2m}t}$$
* **Physical Behavior:** The system returns to equilibrium as fast as possible without oscillating. This is the ideal tuning for systems like car shock absorbers.

**Case 3: Overdamped ($b^2 - 4mk > 0$, or $b > 2\sqrt{mk}$)**
* **Mathematical Result:** The roots are real, distinct, and negative.
* **General Solution:** $$x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}$$
* **Physical Behavior:** Damping is so strong that the system slowly "creeps" back toward equilibrium without ever oscillating. It takes longer to reach equilibrium than the critically damped case.
