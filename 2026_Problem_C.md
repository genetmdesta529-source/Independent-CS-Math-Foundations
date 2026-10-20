### Mathematical Evaluation: Problem C (Analytical Computation)

#### Problem Statement
Determine the numerical value of the following expression without the use of a calculator:
$$\log_4(64) - \frac{(-1)^{2026}}{2} + \sum_{k=1}^{4} \frac{\cos\left(\frac{\pi}{2} + k\pi\right)}{(-1)^{k+1}} + \sqrt{\left(3\sqrt{3}\right)^2} - 1$$

#### Step-by-Step Deconstruction & Evaluation

To evaluate this expression rigorously, we can break it down into five individual components:

**Component 1: The Logarithmic Term**
Using base properties of logarithms where $64 = 4^3$:
$$\log_4(64) = \log_4(4^3) = 3\log_4(4) = 3(1) = 3$$

**Component 2: The Even Power Term**
Since $2026$ is an even integer, $(-1)^{2026} = 1$. Therefore:
$$- \frac{(-1)^{2026}}{2} = - \frac{1}{2}$$

**Component 3: The Finite Trigonometric Summation**
Let's evaluate the term inside the summation $\sum_{k=1}^{4}$ for each value of $k$. Using the trigonometric identity $\cos\left(\frac{\pi}{2} + \theta\right) = -\sin(\theta)$, we can simplify the numerator to $\cos\left(\frac{\pi}{2} + k\pi\right) = -\sin(k\pi)$. 
Since $\sin(k\pi) = 0$ for all integer values of $k$:
$$\cos\left(\frac{\pi}{2} + k\pi\right) = 0 \quad \text{for } k = 1, 2, 3, 4$$

Because the numerator of every single term in the sum is $0$, the entire summation collapses to zero:
$$\sum_{k=1}^{4} \frac{0}{(-1)^{k+1}} = 0$$

**Component 4: The Radical Term**
By the definition of principal square roots, $\sqrt{a^2} = |a|$. Since $3\sqrt{3}$ is positive:
$$\sqrt{\left(3\sqrt{3}\right)^2} = 3\sqrt{3}$$

**Component 5: The Constant Integer**
The trailing constant is simply:
$$-1$$

#### Synthesis of Component Values
Substituting our individual evaluations back into the global expression:
$$\text{Value} = 3 - \frac{1}{2} + 0 + 3\sqrt{3} - 1$$

Combine the rational constant integers and fractions ($3 - 1 - \frac{1}{2}$):
$$2 - \frac{1}{2} + 3\sqrt{3} = \frac{3}{2} + 3\sqrt{3}$$

#### Final Evaluated Solution
The exact numerical value of the expression in simplest radical form is:
$$\mathbf{\frac{3}{2} + 3\sqrt{3}} \quad \text{or} \quad \mathbf{1.5 + 3\sqrt{3}}$$
