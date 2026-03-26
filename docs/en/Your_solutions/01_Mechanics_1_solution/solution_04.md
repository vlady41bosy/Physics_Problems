## 4. Vector Calculus Solutions

To find the velocity and acceleration vectors, we need to take the first and second time derivatives of the position vector, respectively.

* **Find the velocity vector:**
    The velocity vector $\vec{v}(t)$ is the first derivative of the position vector $\vec{r}(t)$ with respect to time $t$. We differentiate the $\hat{i}$ and $\hat{j}$ components individually:
    $$\vec{v}(t) = \frac{d\vec{r}}{dt} = \frac{d}{dt}(3t^2)\hat{i} + \frac{d}{dt}(5t - 8t^2)\hat{j}$$
    $$\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}$$

* **Find the acceleration vector:**
    The acceleration vector $\vec{a}(t)$ is the first derivative of the velocity vector $\vec{v}(t)$ (or the second derivative of the position vector) with respect to time $t$:
    $$\vec{a}(t) = \frac{d\vec{v}}{dt} = \frac{d}{dt}(6t)\hat{i} + \frac{d}{dt}(5 - 16t)\hat{j}$$
    $$\vec{a}(t) = 6\hat{i} - 16\hat{j}$$
    Notice that the acceleration in this case is constant, meaning it does not change as time $t$ progresses.

---
