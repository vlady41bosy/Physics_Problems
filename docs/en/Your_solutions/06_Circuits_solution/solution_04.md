Here is the step-by-step solution to find the equivalent resistance of the mixed circuit shown in the image.

We will break the circuit down from the inside out. Let's designate the resistance of each individual resistor as $R = 10 \text{ \Omega}$.

### **1. Analyze the Circuit Structure**

The circuit splits into two main branches (top and bottom) that run parallel to each other, which then reconnect and pass through a final resistor in series.

* **Top Branch:** Contains two resistors in series.
* **Bottom Branch:** Contains one resistor in series with a parallel pair of resistors.
* **Final Section:** One resistor in series with the rest of the circuit.

### **2. Simplify the Bottom Branch**

First, resolve the small parallel section inside the bottom branch. It consists of two $10 \text{ \Omega}$ resistors in parallel.


$$R_{parallel\_sub} = \frac{R \cdot R}{R + R}$$

$$R_{parallel\_sub} = \frac{10 \cdot 10}{10 + 10}$$

$$R_{parallel\_sub} = \frac{100}{20} = 5 \text{ \Omega}$$

Now, add this to the other resistor in the bottom branch, which is in series with it:


$$R_{bottom} = R + R_{parallel\_sub}$$

$$R_{bottom} = 10 + 5 = 15 \text{ \Omega}$$

### **3. Simplify the Top Branch**

The top branch simply consists of two resistors in series.


$$R_{top} = R + R$$

$$R_{top} = 10 + 10 = 20 \text{ \Omega}$$

### **4. Calculate the Main Parallel Section**

Now we have simplified the circuit to a $20 \text{ \Omega}$ top branch running in parallel with a $15 \text{ \Omega}$ bottom branch. Let's calculate their equivalent resistance ($R_{main\_parallel}$):


$$R_{main\_parallel} = \frac{R_{top} \cdot R_{bottom}}{R_{top} + R_{bottom}}$$

$$R_{main\_parallel} = \frac{20 \cdot 15}{20 + 15}$$

$$R_{main\_parallel} = \frac{300}{35}$$

Divide the numerator and denominator by 5 to simplify the fraction:


$$R_{main\_parallel} = \frac{60}{7} \text{ \Omega}$$

### **5. Calculate Final Equivalent Resistance**

Finally, this entire parallel section is in series with the last $10 \text{ \Omega}$ resistor on the right side of the circuit before the output terminal.


$$R_{eq} = R_{main\_parallel} + R$$

$$R_{eq} = \frac{60}{7} + 10$$

To add these, find a common denominator:


$$R_{eq} = \frac{60}{7} + \frac{70}{7}$$

$$R_{eq} = \frac{130}{7} \text{ \Omega}$$

**Answer:** The equivalent resistance of the circuit is **130/7 Ω**, which is approximately **18.57 Ω**.
