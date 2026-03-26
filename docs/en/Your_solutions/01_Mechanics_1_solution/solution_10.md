## 10. Kinematics Solutions

* **a) Find the equation of the point's trajectory:**
    To find the trajectory equations independent of the parameter $t$, we first examine the $x$ and $y$ components:
    $$x = a \cos(\omega t)$$
    $$y = b \sin(\omega t)$$
    
    We can isolate the trigonometric functions and use the Pythagorean identity $\cos^2(\theta) + \sin^2(\theta) = 1$:
    $$\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = \cos^2(\omega t) + \sin^2(\omega t) = 1$$
    This equation describes an elliptical cylinder extending along the $z$-axis. 
    
    Next, we use the $z$ component to eliminate $t$ entirely. Since $z = bt$, we have $t = \frac{z}{b}$. Substituting this into the original parametric equations gives the exact spatial trajectory:
    $$x(z) = a \cos\left(\frac{\omega z}{b}\right)$$
    $$y(z) = b \sin\left(\frac{\omega z}{b}\right)$$
    The trajectory is an **elliptical helix** winding upward along the surface of the elliptical cylinder $\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = 1$.

* **b) Compute the path length from time $t=0$ to $t=t_0$:**
    The path length $S$ is the integral of the magnitude of the velocity vector over time:
    $$S = \int_{0}^{t_0} |\vec{v}(t)| dt$$
    
    First, find the velocity vector by differentiating the position vector $\vec{r}(t)$ with respect to time:
    $$\vec{v}(t) = \frac{d\vec{r}}{dt} = (-a\omega \sin(\omega t), b\omega \cos(\omega t), b)$$
    
    Now, find the magnitude of the velocity (the speed):
    $$|\vec{v}(t)| = \sqrt{(-a\omega \sin(\omega t))^2 + (b\omega \cos(\omega t))^2 + b^2}$$
    $$|\vec{v}(t)| = \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}$$
    
    Set up the integral for the path length:
    $$S = \int_{0}^{t_0} \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2} \, dt$$
    For the general case where $a \neq b$, this integral does not have a simple closed-form solution in terms of elementary functions and requires evaluation using incomplete elliptic integrals of the second kind.

* **c) Draw the trajectory and discuss special cases:**
    Here is a Python script using `matplotlib` to visualize this 3D trajectory.

```python
import numpy as np
import matplotlib.pyplot as plt

# Define constants
a = 5.0      # x-axis amplitude
b = 3.0      # y-axis amplitude and z-axis velocity factor
omega = 2.0  # angular frequency
t0 = 10.0    # end time

# Generate time array
t = np.linspace(0, t0, 1000)

# Calculate coordinates
x = a * np.cos(omega * t)
y = b * np.sin(omega * t)
z = b * t

# Create 3D plot
fig = plt.figure(figsize=(8, 6))
ax = fig.add_subplot(111, projection='3d')

# Plot the trajectory
ax.plot(x, y, z, label='Elliptical Helix', color='b', linewidth=2)

# Set labels and title
ax.set_xlabel('X axis')
ax.set_ylabel('Y axis')
ax.set_zlabel('Z axis')
ax.set_title('Trajectory of Point M: r(t) = (a*cos(wt), b*sin(wt), bt)')
ax.legend()

plt.show()
```

> **Special Cases Discussion:**
> * **Circular Helix ($a = b$):** If the amplitudes $a$ and $b$ are equal, the base cylinder becomes a perfect circle ($x^2 + y^2 = a^2$). The speed under the integral from part (b) simplifies dramatically because $\sin^2(\omega t) + \cos^2(\omega t) = 1$. The speed becomes constant: $|\vec{v}| = \sqrt{a^2\omega^2 + b^2}$. The path length integral then has a simple closed-form solution: $S = t_0 \sqrt{a^2\omega^2 + b^2}$.
> * **Zero Angular Frequency ($\omega \to 0$):** If the angular frequency approaches zero, the cosine term stays at $1$ and the sine term stays at $0$. The position vector becomes $\vec{r}(t) = (a, 0, bt)$, representing a straight vertical line moving parallel to the $z$-axis at a constant distance $a$ from the origin.

---

