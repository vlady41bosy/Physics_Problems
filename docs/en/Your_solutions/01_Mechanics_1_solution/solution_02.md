## 2. Range Optimization Solutions

To analytically show that the maximum range is achieved at a launch angle of $45^\circ$, we need to find the maximum value of the range function with respect to the angle $\theta$. 

* **State the range function:**
    The range of the projectile is given by the function:
    $$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$
    Here, the initial velocity $v_0$ and the acceleration due to gravity $g$ are constants. The only variable is the launch angle $\theta$.

* **Find the first derivative:**
    To find the extrema (maximums or minimums) of the function, we take the first derivative of $R$ with respect to $\theta$ using the chain rule:
    $$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}[\sin(2\theta)]$$
    $$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta)$$
    $$\frac{dR}{d\theta} = \frac{2v_0^2 \cos(2\theta)}{g}$$

* **Set the derivative to zero:**
    Set the first derivative equal to zero to find the critical points:
    $$\frac{2v_0^2 \cos(2\theta)}{g} = 0$$
    Since the initial velocity $v_0 \neq 0$ and $g \neq 0$, the only way for this equation to be true is if the cosine term is equal to zero:
    $$\cos(2\theta) = 0$$

* **Solve for the angle $\theta$:**
    For a projectile fired over level ground, the practical launch angle is restricted to the interval $0^\circ \leq \theta \leq 90^\circ$. Therefore, $0^\circ \leq 2\theta \leq 180^\circ$. Within this interval, the cosine function is zero only at $90^\circ$:
    $$2\theta = 90^\circ$$
    $$\theta = 45^\circ$$

* **Verify it is a maximum (Second Derivative Test):**
    To confirm this critical point yields a maximum range (and not a minimum), we can take the second derivative of the range function:
    $$\frac{d^2R}{d\theta^2} = \frac{d}{d\theta}\left[\frac{2v_0^2 \cos(2\theta)}{g}\right] = -\frac{4v_0^2 \sin(2\theta)}{g}$$
    Evaluating this at $\theta = 45^\circ$:
    $$\frac{d^2R}{d\theta^2}\bigg|_{\theta=45^\circ} = -\frac{4v_0^2 \sin(90^\circ)}{g} = -\frac{4v_0^2}{g}$$
    Because $v_0^2$ and $g$ are always positive, the second derivative is negative. A negative second derivative confirms that $\theta = 45^\circ$ is a local maximum. 

    Alternatively, by inspecting the original function $R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$, the maximum possible value for the sine function is $1$, which occurs when $\sin(2\theta) = 1 \implies 2\theta = 90^\circ \implies \theta = 45^\circ$.

---

