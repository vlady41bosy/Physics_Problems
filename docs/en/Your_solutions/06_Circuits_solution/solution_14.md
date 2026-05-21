Here is the step-by-step breakdown of the differential equation for a series RLC circuit and its mechanical analogy.

### **1. The RLC Circuit Differential Equation**

To find the differential equation, we start with **Kirchhoff's Voltage Law (KVL)**, which states that the sum of the voltage drops across the components in a closed loop must equal the applied voltage $V(t)$:


$$V_L(t) + V_R(t) + V_C(t) = V(t)$$

We can express the voltage across each component in terms of the charge $Q(t)$ on the capacitor and the current $I(t)$, noting that current is the rate of change of charge ($I = \frac{dQ}{dt}$):

* **Inductor:** $V_L = L \frac{dI}{dt} = L \frac{d^2Q}{dt^2}$
* **Resistor:** $V_R = R I = R \frac{dQ}{dt}$
* **Capacitor:** $V_C = \frac{Q}{C}$

Substituting these into the KVL equation yields the fundamental differential equation for the RLC circuit in terms of charge $Q(t)$:


$$L \frac{d^2Q}{dt^2} + R \frac{dQ}{dt} + \frac{1}{C} Q = V(t)$$



---

### **2. The Damped Harmonic Oscillator Equation**

Now, let's look at a classic mechanical system: a mass attached to a spring with a damper (like a shock absorber), driven by an external force.

According to Newton's Second Law ($\Sigma F = ma$), the sum of the forces (external force $F(t)$, damping force $-b \cdot v$, and spring restoring force $-k \cdot x$) equals mass times acceleration:


$$F(t) - b \frac{dx}{dt} - k x = m \frac{d^2x}{dt^2}$$

Rearranging this into the standard differential form gives:


$$m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + k x = F(t)$$

---

### **3. The Analogies**

By placing the two differential equations side-by-side, the mathematical equivalence is perfectly clear. Both are second-order linear ordinary differential equations. The electrical system behaves exactly like the mechanical system.

| Mechanical System (Damped Oscillator) | Electrical System (RLC Circuit) | Conceptual Analogy |
| --- | --- | --- |
| **Position** ($x$) | **Charge** ($Q$) | The fundamental quantity that is moving or accumulating. |
| **Velocity** ($v = \frac{dx}{dt}$) | **Current** ($I = \frac{dQ}{dt}$) | The rate of flow or movement of the fundamental quantity. |
| **Mass** ($m$) | **Inductance** ($L$) | **Inertia:** Mass resists changes in velocity; an inductor resists changes in current. |
| **Damping Coefficient** ($b$) | **Resistance** ($R$) | **Dissipation:** Friction/damping removes energy as heat; resistance removes electrical energy as heat. |
| **Spring Constant** ($k$) | **Inverse Capacitance** ($\frac{1}{C}$) | **Restoring Force/Storage:** A stiff spring (high $k$) stores mechanical energy; a small capacitor (high $\frac{1}{C}$) strongly pushes back against stored charge. |
| **External Force** ($F$) | **Voltage Source** ($V$) | The external "push" driving the system. |
