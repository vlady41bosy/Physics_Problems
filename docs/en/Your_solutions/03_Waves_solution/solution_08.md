Here is the step-by-step mathematical evaluation of each function.

To determine if a function describes a traveling wave, we must check if it satisfies the standard 1D wave equation:
$$\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2}\frac{\partial^2 y}{\partial t^2}$$

*Note: As a general rule, any well-behaved function that can be written entirely in the form $f(x - vt)$ or $f(x + vt)$ will satisfy this equation.*

Let's test each option by finding their second partial derivatives.

---

### **a) $y(x,t) = A\cos(kx^2 - \omega t)$**

**1. Find the second derivative with respect to $x$:**
* First derivative: $\frac{\partial y}{\partial x} = -A\sin(kx^2 - \omega t) \cdot (2kx)$
* Second derivative (requires the product rule):
    $$\frac{\partial^2 y}{\partial x^2} = -2Ak\sin(kx^2 - \omega t) - 4Ak^2x^2\cos(kx^2 - \omega t)$$

**2. Find the second derivative with respect to $t$:**
* First derivative: $\frac{\partial y}{\partial t} = -A\sin(kx^2 - \omega t) \cdot (-\omega) = A\omega\sin(kx^2 - \omega t)$
* Second derivative:
    $$\frac{\partial^2 y}{\partial t^2} = -A\omega^2\cos(kx^2 - \omega t)$$

**3. Compare:**
If we multiply $\frac{\partial^2 y}{\partial t^2}$ by $\frac{1}{v^2}$, it will only yield a cosine term. However, our spatial derivative ($\frac{\partial^2 y}{\partial x^2}$) contains both a sine term and a cosine term with an $x^2$ coefficient. Therefore, they are not proportional.
* **Conclusion:** This **does not** satisfy the wave equation. (The $x^2$ inside the argument ruins the required $x \pm vt$ linear relationship).

---

### **b) $y(x,t) = A(x - vt)^2$**

**1. Find the second derivative with respect to $x$:**
* First derivative: $\frac{\partial y}{\partial x} = 2A(x - vt) \cdot 1$
* Second derivative: 
    $$\frac{\partial^2 y}{\partial x^2} = 2A$$

**2. Find the second derivative with respect to $t$:**
* First derivative: $\frac{\partial y}{\partial t} = 2A(x - vt) \cdot (-v) = -2Av(x - vt)$
* Second derivative: 
    $$\frac{\partial^2 y}{\partial t^2} = -2Av(-v) = 2Av^2$$

**3. Compare:**
Substitute both into the wave equation:
$$2A = \frac{1}{v^2}(2Av^2)$$
$$2A = 2A$$
* **Conclusion:** This **does** satisfy the wave equation.

---

### **c) $y(x,t) = A\log(x + vt)$**

**1. Find the second derivative with respect to $x$:**
* First derivative: $\frac{\partial y}{\partial x} = \frac{A}{x + vt}$
* Second derivative: 
    $$\frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x + vt)^2}$$

**2. Find the second derivative with respect to $t$:**
* First derivative: $\frac{\partial y}{\partial t} = \frac{A}{x + vt} \cdot v = \frac{Av}{x + vt}$
* Second derivative: 
    $$\frac{\partial^2 y}{\partial t^2} = -\frac{Av \cdot v}{(x + vt)^2} = -\frac{Av^2}{(x + vt)^2}$$

**3. Compare:**
Substitute both into the wave equation:
$$-\frac{A}{(x + vt)^2} = \frac{1}{v^2}\left(-\frac{Av^2}{(x + vt)^2}\right)$$
$$-\frac{A}{(x + vt)^2} = -\frac{A}{(x + vt)^2}$$
* **Conclusion:** This **does** satisfy the wave equation.

---

### **Final Answer**
Mathematically, functions **(b)** and **(c)** describe traveling waves because they perfectly satisfy the wave equation. 

*(Physics Note: While mathematically valid, a real, physical wave on a string or in air must be bounded and finite. Function (b) grows to infinity, and function (c) has a singularity, meaning they are mathematical solutions rather than practical physical examples like sine or cosine waves).*
