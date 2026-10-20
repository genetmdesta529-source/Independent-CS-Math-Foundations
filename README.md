### Mathematical Analysis: Real Roots Portfolio

#### Problem Statement
Find all real roots of the function:
$$g(x) = (x - 1) \cdot (x + 4) \cdot (\ln x)$$

#### 1. Domain Restriction Analysis
Before solving for individual factors, we must establish the natural domain of the function $g(x)$. The natural logarithm function $\ln x$ is strictly defined for positive real numbers:
$$\text{Domain: } x \in (0, \infty) \quad \text{or} \quad x > 0$$

Any solution candidate failing to satisfy this constraint must be discarded as an extraneous solution.

#### 2. Root Calculation by Factorization
By the Zero Product Property, $g(x) = 0$ if and only if at least one of its algebraic constituent factors is equal to zero:

1. **First Linear Factor:**
   $$x - 1 = 0 \implies x = 1$$
   *Domain Verification:* $1 > 0$ (Valid Solution)

2. **Second Linear Factor:**
   $$x + 4 = 0 \implies x = -4$$
   *Domain Verification:* $-4 \ngtr 0$. The evaluation of $\ln(-4)$ yields an undefined value over the field of real numbers $\mathbb{R}$. Thus, $x = -4$ is an extraneous solution.

3. **Logarithmic Factor:**
   $$\ln x = 0 \implies x = e^0 \implies x = 1$$
   *Domain Verification:* $1 > 0$ (Valid Solution)

#### Final Solution Set
Intersecting our candidate solutions with our domain boundary leaves a single element. The function possesses exactly one unique real root:
$$\mathbf{x = 1}$$

IYMC Qualification Round 2026
Problem A
Find all real roots of the function g(x) = (x − 1) · (x + 4) · (ln x).
