
Think of Alice and Bob as two people walking along two different straight paths in a giant park. We need to figure out if their walking paths ever cross, if they bump into each other, and if not, how close they get.

Here is the step-by-step way to solve and understand this problem.

### Step 1: Do their paths cross? (The Intersection)


First, we just want to know if the "roads" they are walking on cross each other. They could reach this crossing point at completely different times of the day, so we have to give them separate stopwatches: $t_A$ for Alice and $t_B$ for Bob.

To find out if the paths cross, we see if there is an $(x, y)$ location that exists on both paths. We set their $x$-coordinates and $y$-coordinates equal to each other:
$$2 + t_A = 2t_B - 1$$
$$8 - 3t_A = 2t_B + 2$$

Now, we solve for the times. From the first equation, we can see that $t_A = 2t_B - 3$. If we plug that into the second equation:
$$8 - 3(2t_B - 3) = 2t_B + 2$$
$$8 - 6t_B + 9 = 2t_B + 2$$
$$17 - 6t_B = 2t_B + 2$$
$$15 = 8t_B$$

This gives us Bob's time at the crossing point: **1.875**. 
If we plug 1.875 back into Alice's equation ($t_A = 2(1.875) - 3$), we get Alice's time: **0.75**.

**Conclusion:** Because both stopwatches show real times, **yes, their paths intersect**. If you plug those times back into the very first coordinate equations, you will find the exact crossing point on the map is **(2.75, 5.75)**.

---

### Step 2: Do they bump into each other? (The Collision)
For a collision to happen, Alice and Bob must arrive at that exact crossing point at the *exact same time*. Now, they share the same stopwatch, so we just use $t$.

Let's test if this is possible by setting their $x$ and $y$ coordinates equal using the same $t$:
* **X-coordinates:** $2 + t = 2t - 1$ (This solves to $t = 3$)
* **Y-coordinates:** $8 - 3t = 2t + 2$ (This solves to $t = 1.2$)

**Conclusion:** Alice reaches the crossing point when the stopwatch says 1.2, but Bob doesn't get there until the stopwatch says 3. Since they are there at different times, **they do not collide**. 

---

### Step 3: What is their closest call? (Minimum Distance)


Since they miss each other, we want to find out exactly how close they were at their nearest point. To do this, we use the standard distance formula between two points. 

To make the calculus much easier, we calculate the *squared* distance, written as $D^2(t)$, so we don't have to deal with messy square roots right away. We subtract Alice's coordinates from Bob's coordinates:
* Distance between their $x$-positions: $(2t - 1) - (2 + t) = t - 3$
* Distance between their $y$-positions: $(2t + 2) - (8 - 3t) = 5t - 6$

Now, we square those and add them together:
$$D^2(t) = (t - 3)^2 + (5t - 6)^2$$
$$D^2(t) = (t^2 - 6t + 9) + (25t^2 - 60t + 36)$$
$$D^2(t) = 26t^2 - 66t + 45$$

To find the exact moment they are closest (the absolute minimum of this equation), we take the first derivative and set it to zero:
$$\frac{d}{dt}[D^2(t)] = 52t - 66$$
$$0 = 52t - 66$$

Solving this gives us $t = \frac{66}{52}$, which simplifies to $\frac{33}{26}$ (or about **1.27**). This is the exact time they are closest to each other!

Finally, we plug that time back into our squared distance formula:
$$D^2\left(\frac{33}{26}\right) = \frac{81}{26}$$

**Conclusion:** To get the actual minimum distance, we just take the square root of that final number. $\sqrt{\frac{81}{26}}$ gives us roughly **1.765 units of distance**.

---
