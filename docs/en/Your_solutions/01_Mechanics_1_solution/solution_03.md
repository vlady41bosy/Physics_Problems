## 3. Path Intersection Solutions

To solve this problem completely, we must distinguish between the *paths* intersecting (crossing the same point in space at any time) and the *objects* colliding (arriving at the exact same point in space at the exact same time).

* **Determine if the paths intersect:**
    To find if the geometric lines cross, we need to see if there is a coordinate $(x, y)$ that lies on both paths. This means Alice reaches the point at some time $t_A$ and Bob reaches it at some time $t_B$. We set their coordinate equations equal to each other:
    $$x_A(t_A) = x_B(t_B) \implies 2 + t_A = 2t_B - 1$$
    $$y_A(t_A) = y_B(t_B) \implies 8 - 3t_A = 2t_B + 2$$
    
    From the $x$-equation, we can isolate $t_A$:
    $$t_A = 2t_B - 3$$
    
    Substitute this into the $y$-equation:
    $$8 - 3(2t_B - 3) = 2t_B + 2$$
    $$8 - 6t_B + 9 = 2t_B + 2$$
    $$17 - 6t_B = 2t_B + 2$$
    $$15 = 8t_B \implies t_B = \frac{15}{8} = 1.875$$
    
    Now solve for $t_A$:
    $$t_A = 2(1.875) - 3 = 3.75 - 3 = 0.75$$
    
    Because we found valid, real times for both variables, **yes, their paths intersect**. By plugging these times back into their respective equations, we find the intersection point occurs at $(2.75, 5.75)$.

* **Determine if they collide:**
    A collision requires them to be at the intersection point at the exact same time ($t_A = t_B = t$). We can test this by setting their $x$ and $y$ equations equal to each other using a single time variable $t$:
    $$2 + t = 2t - 1 \implies t = 3$$
    $$8 - 3t = 2t + 2 \implies 5t = 6 \implies t = 1.2$$
    
    Since $3 \neq 1.2$, Alice and Bob arrive at the intersection point at different times. Therefore, **they do not collide**.

* **Determine the minimum distance and when it occurs:**
    Since they do not collide, we need to find the function for the distance $D(t)$ between them at any given time $t$. To make the calculus easier, we will minimize the square of the distance, $D^2(t)$, using the distance formula:
    $$D^2(t) = (x_B(t) - x_A(t))^2 + (y_B(t) - y_A(t))^2$$
    
    First, find the differences in their coordinates:
    $$\Delta x = (2t - 1) - (2 + t) = t - 3$$
    $$\Delta y = (2t + 2) - (8 - 3t) = 5t - 6$$
    
    Now construct the squared distance function:
    $$D^2(t) = (t - 3)^2 + (5t - 6)^2$$
    $$D^2(t) = (t^2 - 6t + 9) + (25t^2 - 60t + 36)$$
    $$D^2(t) = 26t^2 - 66t + 45$$
    
    To find the minimum, take the first derivative with respect to $t$ and set it to zero:
    $$\frac{d}{dt}[D^2(t)] = 52t - 66$$
    $$0 = 52t - 66 \implies t = \frac{66}{52} = \frac{33}{26} \approx 1.269 \text{ units of time}$$
    
    This is the time when they are closest. To find the minimum distance, plug $t = \frac{33}{26}$ back into the $D^2(t)$ function:
    $$D^2\left(\frac{33}{26}\right) = 26\left(\frac{33}{26}\right)^2 - 66\left(\frac{33}{26}\right) + 45$$
    $$D^2\left(\frac{33}{26}\right) = \frac{1089}{26} - \frac{2178}{26} + \frac{1170}{26} = \frac{81}{26}$$
    
    Taking the square root gives the minimum distance:
    $$D = \sqrt{\frac{81}{26}} = \frac{9}{\sqrt{26}} \approx 1.765 \text{ units of distance}$$

---

