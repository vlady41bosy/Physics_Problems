## 7. Elimination of time and interpretation of acceleration Solutions

* **Eliminate the parameter $t$:**
    To find the path equation $y(x)$, we need to relate the $x$ and $y$ equations by removing $t$. 
    First, isolate $t^2$ from the horizontal position equation:
    $$x = 2t^2 \implies t^2 = \frac{x}{2}$$
    To easily substitute this into the $y(t)$ equation, we can manipulate both equations to feature $t^6$. Cube the $x$ relationship and square the $y$ relationship:
    $$(t^2)^3 = \left(\frac{x}{2}\right)^3 \implies t^6 = \frac{x^3}{8}$$
    $$y = 3t^3 \implies y^2 = 9t^6$$
    Substitute the expression for $t^6$ into the squared $y$ equation:
    $$y^2 = 9\left(\frac{x^3}{8}\right) \implies y^2 = \frac{9}{8}x^3$$
    This is the Cartesian equation for the path, which represents a semi-cubical parabola. Note that since $x = 2t^2$, the value of $x$ will always be non-negative.

* **Draw the trajectory:**
    The trajectory is a curve in the $xy$-plane that is symmetric about the x-axis and opens to the right. As $t$ increases from negative values to zero, the object moves from the lower quadrant toward the origin $(0,0)$ along the bottom branch of the curve. As $t$ increases from zero to positive values, the object moves away from the origin into the upper right quadrant along the top branch. 

* **Calculate $\vec{v}(t)$, $|\vec{v}(t)|$, $\vec{a}(t)$ and $|\vec{a}(t)|$:**
    The velocity vector $\vec{v}(t)$ is the first time derivative of the position components:
    $$\vec{v}(t) = \frac{dx}{dt}\hat{i} + \frac{dy}{dt}\hat{j} = 4t\hat{i} + 9t^2\hat{j}$$
    The magnitude of the velocity (speed) $|\vec{v}(t)|$ is found using the Pythagorean theorem:
    $$|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = |t|\sqrt{16 + 81t^2}$$
    The acceleration vector $\vec{a}(t)$ is the first time derivative of the velocity components:
    $$\vec{a}(t) = \frac{dv_x}{dt}\hat{i} + \frac{dv_y}{dt}\hat{j} = 4\hat{i} + 18t\hat{j}$$
    The magnitude of the acceleration $|\vec{a}(t)|$ is:
    $$|\vec{a}(t)| = \sqrt{4^2 + (18t)^2} = \sqrt{16 + 324t^2} = 2\sqrt{4 + 81t^2}$$

* **Is the acceleration constant?**
    No, the acceleration is not constant. While the horizontal component of the acceleration is a constant $4$, the vertical component is $18t$. Because the vertical component depends on the variable $t$, the overall acceleration vector changes continuously over time in both magnitude and direction.

