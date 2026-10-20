### Rigorous Proof: Problem B (Non-Existence of Real Solutions)

#### Problem Statement
Show that there is no $x \in \mathbb{R}$ that solves the equation:
$$\sqrt{3 + x} + \sqrt{7 - x} = 5$$

#### Proof via Function Optimization (Upper Bound Constraints)

**1. Domain Restriction Analysis:**
For the real-valued square root functions to be defined, their radicands must be non-negative:
*   $3 + x \geq 0 \implies x \geq -3$
*   $7 - x \geq 0 \implies x \leq 7$

Thus, any real solution must lie within the bounded interval:
$$\text{Domain: } x \in [-3, 7]$$

**2. Function Definition & Algebraic Squaring:**
Let $f(x) = \sqrt{3 + x} + \sqrt{7 - x}$. To find the maximum possible value this function can achieve on its domain, let's square both sides of the expression:
$$[f(x)]^2 = (\sqrt{3 + x} + \sqrt{7 - x})^2$$
$$[f(x)]^2 = (3 + x) + (7 - x) + 2\sqrt{(3 + x)(7 - x)}$$
$$[f(x)]^2 = 10 + 2\sqrt{21 + 4x - x^2}$$

**3. Maximizing the Radicand:**
To maximize the value of $[f(x)]^2$, we must maximize the quadratic expression inside the radical: $g(x) = -x^2 + 4x + 21$.
The vertex of this downward-opening parabola occurs at:
$$x = -\frac{b}{2a} = -\frac{4}{2(-1)} = 2$$

Since $2 \in [-3, 7]$, the absolute maximum value of $g(x)$ is:
$$g(2) = -(2)^2 + 4(2) + 21 = -4 + 8 + 21 = 25$$

**4. Determining the Global Maximum Bound:**
Substitute $g(2) = 25$ back into our squared function model:
$$\max([f(x)]^2) = 10 + 2\sqrt{25} = 10 + 2(5) = 20$$
$$\max(f(x)) = \sqrt{20} = 2\sqrt{5} \approx 4.472$$

#### Conclusion
Since the maximum possible real value that the expression $\sqrt{3 + x} + \sqrt{7 - x}$ can attain is $2\sqrt{5}$ ($\approx 4.472$), it is mathematically impossible for the function to equal $5$. Therefore, no real solution $x \in \mathbb{R}$ exists. $\blacksquare$
