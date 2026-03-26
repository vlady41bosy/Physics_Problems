## 5. Relative Velocity Solutions

To solve this problem, we use vector addition. The boat's actual velocity relative to the ground is the sum of its velocity in still water and the river's velocity. 

* **Determine the direction (angle) to head:**
    To travel directly north, the boat must head somewhat upstream (west) to exactly counteract the river's eastward current. We can represent these velocities as a right triangle. 
    The river's velocity ($v_r = 2 \text{ m/s}$) points East.
    The boat's velocity in still water ($v_b = 5 \text{ m/s}$) forms the hypotenuse.
    The resulting velocity relative to the shore ($v_{result}$) points directly North.
    
    Let $\theta$ be the angle west of North that the boat must steer. To move straight north, the westward component of the boat's velocity must equal the eastward velocity of the river:
    $$v_b \sin(\theta) = v_r$$
    $$5\sin(\theta) = 2$$
    $$\sin(\theta) = \frac{2}{5} = 0.4$$
    $$\theta = \arcsin(0.4) \approx 23.58^\circ$$
    The boat should head approximately $23.58^\circ$ West of North.

* **Determine the time to cross the river:**
    The time it takes to cross depends entirely on the northward component of the boat's velocity ($v_y$). The eastward and westward velocities cancel out, so they do not help or hinder progress across the width of the river.
    
    Using the Pythagorean theorem on our velocity triangle ($v_y^2 + v_r^2 = v_b^2$), we can find the magnitude of the northward velocity:
    $$v_y = \sqrt{v_b^2 - v_r^2}$$
    $$v_y = \sqrt{5^2 - 2^2} = \sqrt{25 - 4} = \sqrt{21} \approx 4.58 \text{ m/s}$$
    
    Now, use the basic kinematic equation for constant velocity ($d = vt$) to find the time $t$ required to cross the $200 \text{ m}$ distance:
    $$t = \frac{d}{v_y}$$
    $$t = \frac{200}{\sqrt{21}} \approx \frac{200}{4.583} \approx 43.64 \text{ s}$$

---

