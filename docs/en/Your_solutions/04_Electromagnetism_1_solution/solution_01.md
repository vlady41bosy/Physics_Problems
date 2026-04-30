

### **1. Identify the Given Information**
*   **Corner charges ($q_1, q_2, q_3, q_4$):** $+1.0 \text{ C}$ each.
*   **Center charge ($q_0$):** $-2.0 \text{ C}$.
*   **Side length of the square ($a$):** $1.0 \text{ m}$.
*   **Coulomb's constant ($k$):** $8.99 \times 10^9 \text{ N}\cdot\text{m}^2/\text{C}^2$.

### **2. Calculate the Distance ($r$)**
First, we need the exact distance from any corner of the square to the center.
*   The diagonal ($d$) of a square is calculated using the Pythagorean theorem: $d = a\sqrt{2}$.

      $$d = 1.0\sqrt{2} \text{ m}$$
*   The distance from a corner to the center ($r$) is exactly half of the diagonal:

    $$r = \frac{1.0\sqrt{2}}{2} \text{ m}$$
*   For Coulomb's Law, we need $r^2$:

      $$r^2 = \left(\frac{\sqrt{2}}{2}\right)^2 = \frac{2}{4} = 0.5 \text{ m}^2$$

### **3. Calculate the Magnitude of the Force from One Corner**
Using Coulomb's Law, we find the magnitude of the force exerted by *one* of the $+1.0 \text{ C}$ corner charges on the central $-2.0 \text{ C}$ charge. We only use the absolute values of the charges for the magnitude.


$$F = k \frac{|q_{\text{corner}} \cdot q_{\text{center}}|}{r^2}$$

$$F = (8.99 \times 10^9) \frac{|1.0 \cdot (-2.0)|}{0.5}$$

$$F = (8.99 \times 10^9) \frac{2.0}{0.5}$$

$$F = (8.99 \times 10^9) \cdot 4$$

$$F = 3.596 \times 10^{10} \text{ N}$$

Because all four corner charges have the exact same magnitude ($+1.0 \text{ C}$) and are at the exact same distance ($r$), the magnitude of the force from *each* corner is identical: $3.596 \times 10^{10} \text{ N}$.

### **4. Vector Addition (The Direction)**
Force is a vector, meaning direction matters. 
Let's label the corners: **Top-Left (1), Top-Right (2), Bottom-Right (3), and Bottom-Left (4).**

*   Because opposite charges attract, the negative center charge is pulled **towards** each positive corner.
*   **Force 1 ($\vec{F}_1$)** pulls the center charge towards the Top-Left.
*   **Force 3 ($\vec{F}_3$)** pulls the center charge towards the Bottom-Right.
*   Since $\vec{F}_1$ and $\vec{F}_3$ have the exact same magnitude but pull in exactly **opposite directions**, they cancel each other out perfectly: 
    $$\vec{F}_1 + \vec{F}_3 = 0$$
*   Similarly, **Force 2 ($\vec{F}_2$)** pulling towards the Top-Right is perfectly canceled by **Force 4 ($\vec{F}_4$)** pulling towards the Bottom-Left: 
    $$\vec{F}_2 + \vec{F}_4 = 0$$

### **Conclusion**
To find the total net force ($\vec{F}_{\text{net}}$), we add all the force vectors together:

$$\vec{F}_{\text{net}} = \vec{F}_1 + \vec{F}_2 + \vec{F}_3 + \vec{F}_4$$

$$\vec{F}_{\text{net}} = (\vec{F}_1 + \vec{F}_3) + (\vec{F}_2 + \vec{F}_4)$$

$$\vec{F}_{\text{net}} = 0 \text{ N} + 0 \text{ N} = 0 \text{ N}$$

**Final Answer:** The net magnitude is **$0 \text{ N}$**. Because the net force is exactly zero, there is **no direction**.
