# Solutions goes here



## 1. Projectile Motion Solutions

* **Derive the differential equations of motion in the horizontal and vertical directions:**
    By applying Newton's Second Law ($\Sigma F = ma$), we look at the forces acting on the projectile once it is in the air. Assuming no air resistance, the only force acting on the object is gravity pulling it downward.
    
    In the horizontal ($x$) direction, there are no forces:
    $$F_x = m \frac{d^2x}{dt^2} = 0 \implies \frac{d^2x}{dt^2} = 0$$
    
    In the vertical ($y$) direction, the force of gravity acts downward:
    $$F_y = m \frac{d^2y}{dt^2} = -mg \implies \frac{d^2y}{dt^2} = -g$$

* **Determine the time of flight:**
    First, establish the initial velocity components:
    $v_{0x} = 100 \cos(37^\circ) \approx 100(0.8) = 80 \text{ m/s}$
    $v_{0y} = 100 \sin(37^\circ) \approx 100(0.6) = 60 \text{ m/s}$

    Integrating the vertical differential equation gives us the position equation $y(t) = v_{0y}t - \frac{1}{2}gt^2$. The projectile lands when $y = 0$:
    $$0 = t(v_{0y} - \frac{1}{2}gt)$$
    Solving for $t$ (ignoring $t = 0$ as the launch time) gives the time of flight $T$:
    $$T = \frac{2v_{0y}}{g} = \frac{2(60)}{9.8} \approx 12.24 \text{ s}$$

* **Determine the maximum height:**
    Maximum height occurs when the vertical velocity is zero ($v_y = 0$). Integrating the vertical acceleration gives the velocity equation $v_y(t) = v_{0y} - gt$. Setting $v_y = 0$:
    $$0 = v_{0y} - gt \implies t_{max} = \frac{v_{0y}}{g}$$
    Substitute this time back into the vertical position equation to get the maximum height $H$:
    $$H = v_{0y}\left(\frac{v_{0y}}{g}\right) - \frac{1}{2}g\left(\frac{v_{0y}}{g}\right)^2 = \frac{v_{0y}^2}{2g}$$
    $$H = \frac{60^2}{2(9.8)} = \frac{3600}{19.6} \approx 183.67 \text{ m}$$

* **Determine the range:**
    The range is the horizontal distance traveled during the total time of flight $T$. Integrating the horizontal differential equation gives the position equation $x(t) = v_{0x}t$. Substituting the time of flight $T$:
    $$R = v_{0x}T = v_{0x}\left(\frac{2v_{0y}}{g}\right)$$
    $$R = 80 \times 12.24 \approx 979.2 \text{ m}$$

---


...
