To find all the possible equivalent resistances, we have to look at all the different ways we can wire these identical $1\ \Omega$ resistors together.

Usually, this classic problem implies using **all three** resistors in the circuit, so let's start with those four unique combinations. Then, I'll also list the values you can get if you're allowed to leave one or two resistors in the box.

### **Combinations Using All 3 Resistors**

**1. All Three in Series**
When connected end-to-end, the resistances simply add up.

* **Formula:** $R = R_1 + R_2 + R_3$
* **Calculation:** $1 + 1 + 1 = 3$
* **Result:** **$3\ \Omega$**

**2. All Three in Parallel**
When all three are connected side-by-side, the current splits three ways.

* **Formula:** $\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$
* **Calculation:** $\frac{1}{R_{eq}} = 1 + 1 + 1 = 3$
* **Result:** **$\frac{1}{3}\ \Omega$** (approx. $0.33\ \Omega$)

**3. Two in Parallel, Series with the Third**
First, put two resistors in parallel. Their equivalent resistance is $\frac{1}{2}\ \Omega$. Then, connect that pair in series with the final $1\ \Omega$ resistor.

* **Calculation:** $0.5 + 1 = 1.5$
* **Result:** **$1.5\ \Omega$** (or $\frac{3}{2}\ \Omega$)

**4. Two in Series, Parallel with the Third**
First, put two resistors in series. Their equivalent resistance is $2\ \Omega$. Then, connect that pair in parallel with the final $1\ \Omega$ resistor.

* **Formula:** $\frac{1}{R_{eq}} = \frac{1}{2} + \frac{1}{1}$
* **Calculation:** $\frac{1}{R_{eq}} = \frac{1}{2} + \frac{2}{2} = \frac{3}{2}$
* **Result:** **$\frac{2}{3}\ \Omega$** (approx. $0.67\ \Omega$)

---

### **Combinations Using Fewer Than 3 Resistors**

If the rules allow you to use a subset of your supply, you can create three more unique values:

**5. Two in Series** (Leaving one unused)

* **Result:** **$2\ \Omega$**

**6. Two in Parallel** (Leaving one unused)

* **Result:** **$0.5\ \Omega$** (or $\frac{1}{2}\ \Omega$)

**7. Just One Resistor** (Leaving two unused)

* **Result:** **$1\ \Omega$**

### **The Final List**

If you must use exactly three resistors, you can create **4 unique values**:

* **$3\ \Omega, 1.5\ \Omega, \frac{2}{3}\ \Omega, \frac{1}{3}\ \Omega$**

If you can use *up to* three resistors, you can create a total of **7 unique values**:

* **$3\ \Omega, 2\ \Omega, 1.5\ \Omega, 1\ \Omega, \frac{2}{3}\ \Omega, 0.5\ \Omega, \frac{1}{3}\ \Omega$**
