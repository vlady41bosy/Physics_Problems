

## 7. Logic & Series: The Fly and the Bicycle (Step-by-Step)

**The Setup:**

* **Bicycle:** 10m from the wall, moving at **1 m/s**.
* **Fly:** Starts at the bicycle, flies toward the wall at **2 m/s**, then turns back and forth.
* **Goal:** Find the total distance the fly travels before it gets crushed.

### Step 1: The "Simple" Perspective (Time)

Instead of trying to calculate every single short trip the fly takes back and forth, just ask yourself: **"How long is the fly in the air?"**

The fly stops flying the exact moment the bicycle hits the wall.

* Distance to wall = 10 meters
* Bicycle speed = 1 m/s
* **Time ($t$):** $10\text{ m} / 1\text{ m/s} = \mathbf{10\text{ seconds}}$

### Step 2: Calculate the Fly's Distance

The fly travels at a constant speed of **2 m/s** for those entire 10 seconds. It doesn't matter how many times it turns around; its speed relative to the ground is always 2 m/s.

* Fly Speed ($v$) = 2 m/s
* Time ($t$) = 10 s
* **Distance ($d$):** $v \cdot t = 2\text{ m/s} \cdot 10\text{ s} = \mathbf{20\text{ meters}}$

**Result:**
The fly travels exactly **20 meters**.

---

## 8. Definite Integrals (Step-by-Step)

**The Problem:**
Calculate the area under $f(x) = \sin(x)$ from $x=0$ to $x=\pi$.

### Step 1: Set up the Integral

To find the area under a curve, we integrate the function between the two given points:


$$\text{Area} = \int_{0}^{\pi} \sin(x) \, dx$$

### Step 2: Find the Antiderivative

The derivative of $\cos(x)$ is $-\sin(x)$, so the antiderivative (integral) of $\sin(x)$ is **$-\cos(x)$**.


$$[-\cos(x)]_{0}^{\pi}$$

### Step 3: Evaluate at the Boundaries

We subtract the value at the bottom boundary (0) from the value at the top boundary ($\pi$):

1. **Top:** $-\cos(\pi) = -(-1) = 1$
2. **Bottom:** $-\cos(0) = -(1) = -1$

Now, subtract them:


$$1 - (-1) = 1 + 1 = \mathbf{2}$$

**Result:**
The total area is exactly **2 square units**.
