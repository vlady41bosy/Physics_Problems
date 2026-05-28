## 3. Mixed Circuit

We are calculating the total equivalent resistance of a complex mixed circuit. By carefully tracing the nodes, we can identify 8 distinct resistors (all 5 Ω). The circuit cannot be solved using simple series/parallel rules alone because it contains a bridge-like structure. We will use a Delta-Wye ($\Delta$-Y) Transformation to simplify it.

---

### Part A: Network Topology

Let's label the input terminals as Node L (left) and Node R (right).
* There is a bottom resistor connected directly between Node L and Node R. We will set this aside and solve the entire "upper" network first.
* On the far left, a vertical resistor and a top horizontal resistor are connected in series since they meet at a corner with no other branching connections. Their combined resistance is $5 + 5 = 10 \ \Omega$.
* The center of the circuit contains a delta ($\Delta$) loop formed by three 5 Ω resistors: the top-middle vertical, the bottom-middle vertical, and the top-right vertical.

### Part B: Delta-Wye Transformation

We convert the central delta ($\Delta$) into a wye (Y) configuration. Since all three resistors in the delta are 5 Ω, the three new resistors in the wye configuration ($R_Y$) will be equal. 

The formula for converting identical delta resistors to a wye network is:

$$
R_Y = \frac{R_\Delta \cdot R_\Delta}{R_\Delta + R_\Delta + R_\Delta} = \frac{R_\Delta}{3}
$$

$$
R_Y = \frac{5}{3} \ \Omega
$$

Replacing the delta with a central wye node (let's call it Node W) breaks the complex bridge into simpler series and parallel branches that we can easily calculate.

### Part C: Solving the Upper Network

Now we calculate the equivalent resistance of the upper network ($R_{upper}$) using the new wye resistors:

1. Parallel Branches to Node W:
From Node L, the current splits into two parallel branches to reach the new Node W:
* Branch 1: Goes through the 10 Ω series combination, then through one $5/3 \ \Omega$ wye resistor.
    $$R_{branch1} = 10 + \frac{5}{3} = \frac{35}{3} \ \Omega$$
* Branch 2: Goes through the inner-horizontal 5 Ω resistor, then through another $5/3 \ \Omega$ wye resistor.
    $$R_{branch2} = 5 + \frac{5}{3} = \frac{20}{3} \ \Omega$$

Now we calculate the equivalent resistance of these two parallel branches ($R_p$):
$$
R_p = \frac{\frac{35}{3} \cdot \frac{20}{3}}{\frac{35}{3} + \frac{20}{3}} = \frac{\frac{700}{9}}{\frac{55}{3}} = \frac{140}{33} \ \Omega
$$

2. Series Path to Node R:
From Node W, the path continues through the third $5/3 \ \Omega$ wye resistor, and then through the bottom-right vertical 5 Ω resistor to reach the final right terminal.
$$
R_{series} = \frac{5}{3} + 5 = \frac{20}{3} = \frac{220}{33} \ \Omega
$$

3. Total Upper Network:
By adding the parallel section to the series section, we get the total resistance for everything above the bottom wire:

$$

R_{upper} = R_p + R_{series} = \frac{140}{33} + \frac{220}{33} = \frac{360}{33} = \frac{120}{11} \ \Omega

$$

### Part D: Total Equivalent Resistance

Finally, the entire upper network is in parallel with the 5 Ω bottom resistor. 

$$
R_{eq} = \frac{R_{upper} \cdot 5}{R_{upper} + 5}
$$

$$
R_{eq} = \frac{\frac{120}{11} \cdot 5}{\frac{120}{11} + 5} = \frac{\frac{600}{11}}{\frac{175}{11}}
$$

$$
R_{eq} = \frac{600}{175} = \frac{24}{7} \ \Omega
$$

### Final Answer

* The equivalent resistance of the entire mixed circuit is exactly 24/7 Ω.
* In decimal form, this is approximately 3.43 Ω.
