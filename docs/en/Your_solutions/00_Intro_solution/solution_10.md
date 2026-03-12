## 10. Infinite Series: The Ant's Journey (Step-by-Step)

This last one looks like a mess of directions, but it’s actually two separate math patterns (one for East/West and one for North/South).

**The Movement:** 1m E, 1/2m N, 1/3m W, 1/4m S, 1/5m E...

### Step 1: Track the X-axis (East/West)

The ant goes East (+), then West (-), then East (+).


$$X = 1 - 1/3 + 1/5 - 1/7 + \dots$$


This is a famous calculus series (the Gregory-Leibniz series) that equals **$\frac{\pi}{4}$**.

### Step 2: Track the Y-axis (North/South)

The ant goes North (+), then South (-), then North (+).


$$Y = 1/2 - 1/4 + 1/6 - 1/8 + \dots$$


If we factor out a $1/2$, it looks like this: $\frac{1}{2}(1 - 1/2 + 1/3 - 1/4 \dots)$.
The part in the parentheses is the natural log of 2 ($\ln(2)$). So the result is **$\frac{\ln(2)}{2}$**.

**Final Result:**
The ant's final position is **$(\frac{\pi}{4}, \frac{\ln(2)}{2})$**, or approximately **(0.785, 0.347)**.
