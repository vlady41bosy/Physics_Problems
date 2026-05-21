

Imagine connecting a battery across two opposite corners of the cube (let's call the entrance corner **A** and the exit corner **B**). Let the total current entering corner A be $I$.

Here is the step-by-step breakdown of how the current flows through the edges (resistors) of the cube to get to corner B:

**1. The First Split (Leaving A)**
When the total current $I$ enters node A, it has three identical edges it can travel along. Because the cube is perfectly symmetrical, the current splits equally three ways.

* Current in each of these 3 initial edges = $\frac{I}{3}$

**2. The Second Split (Middle Edges)**
At the end of each of those first three edges, the current reaches a new node. From each of these nodes, there are two identical paths leading forward toward the exit B. Again, by symmetry, the current splits equally in two.

* Current in each of these 6 middle edges = $\frac{I}{3} \div 2 = \frac{I}{6}$

**3. The Recombination (Approaching B)**
Now, the currents arrive at the three nodes adjacent to the exit corner B. At each of these nodes, two paths carrying $\frac{I}{6}$ merge together to head down the final edge toward B.

* Current in each of these 3 final edges = $\frac{I}{6} + \frac{I}{6} = \frac{I}{3}$
*(These three $\frac{I}{3}$ currents then meet at corner B to perfectly reform the total current $I$).*

**4. Calculating the Voltage Drop**
To find the equivalent resistance, we need to trace **one single path** from A to B and calculate the total voltage drop ($V = I \cdot R$) along that specific route.

No matter which path you choose, it will consist of one initial edge, one middle edge, and one final edge:

* Voltage drop on the first edge: $V_1 = \left(\frac{I}{3}\right) \cdot R$
* Voltage drop on the middle edge: $V_2 = \left(\frac{I}{6}\right) \cdot R$
* Voltage drop on the final edge: $V_3 = \left(\frac{I}{3}\right) \cdot R$

Total voltage drop from A to B:


$$V_{\text{total}} = V_1 + V_2 + V_3$$

$$V_{\text{total}} = \frac{I \cdot R}{3} + \frac{I \cdot R}{6} + \frac{I \cdot R}{3}$$

To add these fractions, find the common denominator (6):


$$V_{\text{total}} = I \cdot R \cdot \left(\frac{2}{6} + \frac{1}{6} + \frac{2}{6}\right)$$

$$V_{\text{total}} = I \cdot R \cdot \left(\frac{5}{6}\right)$$

**5. Finding Equivalent Resistance ($R_{eq}$)**
Ohm's law states that $V_{\text{total}} = I \cdot R_{eq}$. Therefore:


$$I \cdot R_{eq} = I \cdot \left(\frac{5}{6} R\right)$$

**Answer:**
The equivalent resistance between two opposite corners of the cube is **$\frac{5}{6} R$**.
