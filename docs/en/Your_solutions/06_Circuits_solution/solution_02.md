Here is the step-by-step mathematical breakdown for every possible way to arrange exactly three identical $1 \text{ \Omega}$ resistors.

There are exactly four distinct ways to connect three resistors in a circuit:

**1. All Three in Series**
In this configuration, the current passes through each resistor one after the other. We simply add their values.


$$R_{eq} = R_1 + R_2 + R_3$$

$$R_{eq} = 1 + 1 + 1$$

$$R_{eq} = 3 \text{ \Omega}$$

**2. All Three in Parallel**
In this configuration, the resistors are placed on separate branches, meaning the current splits among them.


$$\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$$

$$\frac{1}{R_{eq}} = \frac{1}{1} + \frac{1}{1} + \frac{1}{1}$$

$$\frac{1}{R_{eq}} = 3$$

$$R_{eq} = \frac{1}{3} \text{ \Omega} \approx 0.33 \text{ \Omega}$$

**3. Two in Parallel, Connected in Series with the Third**
First, current splits between two parallel resistors, then the combined current passes through the final resistor.

* Calculate the parallel pair:

$$R_{parallel} = \frac{1}{\frac{1}{1} + \frac{1}{1}} = \frac{1}{2} \text{ \Omega}$$


* Add the third resistor in series:

$$R_{eq} = \frac{1}{2} + 1$$


$$R_{eq} = \frac{3}{2} \text{ \Omega} = 1.5 \text{ \Omega}$$



**4. Two in Series, Connected in Parallel with the Third**
Here, one branch has two resistors in series, and the second branch has just one resistor.

* Calculate the series branch:

$$R_{series} = 1 + 1 = 2 \text{ \Omega}$$


* Calculate the parallel combination of that branch with the third resistor:

$$R_{eq} = \frac{1}{\frac{1}{2} + \frac{1}{1}}$$


$$R_{eq} = \frac{1}{\frac{3}{2}}$$


$$R_{eq} = \frac{2}{3} \text{ \Omega} \approx 0.67 \text{ \Omega}$$



---

### **Final List of Unique Values**

By combining exactly three $1 \text{ \Omega}$ resistors, you can create the following four equivalent resistances:

* **$3 \text{ \Omega}$**
* **$1.5 \text{ \Omega}$** (or $\frac{3}{2} \text{ \Omega}$)
* **$0.67 \text{ \Omega}$** (or $\frac{2}{3} \text{ \Omega}$)
* **$0.33 \text{ \Omega}$** (or $\frac{1}{3} \text{ \Omega}$)
