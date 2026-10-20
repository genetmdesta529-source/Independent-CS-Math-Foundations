### Mathematical Analysis: Problem B

#### Problem Statement
Find all integers $n$ such that the following equation holds true:
$$2^n + 2^{-n} = \frac{5}{2}$$

#### Step-by-Step Algebraic Solution

**1. Algebraic Substitution:**
To simplify the exponential equation, we can use substitution. Let $x = 2^n$. Since $2^n$ must always be strictly positive, we establish the constraint that $x > 0$. 

Rewriting the equation in terms of $x$:
$$x + \frac{1}{x} = \frac{5}{2}$$

**2. Conversion to Quadratic Form:**
Multiply every term by $2x$ to clear the denominators:
$$2x\left(x + \frac{1}{x}\right) = 2x\left(\frac{5}{2}\right)$$
$$2x^2 + 2 = 5x$$

Rearrange the terms into standard quadratic form ($ax^2 + bx + c = 0$):
$$2x^2 - 5x + 2 = 0$$

**3. Factoring the Quadratic Equation:**
We look for two numbers that multiply to $2 \times 2 = 4$ and add up to $-5$. These numbers are $-4$ and $-1$. Splitting the middle term:
$$2x^2 - 4x - x + 2 = 0$$
$$2x(x - 2) - 1(x - 2) = 0$$
$$(2x - 1)(x - 2) = 0$$

This yields two possible values for $x$:
*   $2x - 1 = 0 \implies x = \frac{1}{2}$
*   $x - 2 = 0 \implies x = 2$

Both values satisfy our initial constraint $x > 0$.

**4. Resubstitution to Solve for $n$:**
Now, we substitute $x = 2^n$ back into our solutions to solve for the integer $n$:

*   **Case 1:** $2^n = 2$
    $$2^n = 2^1 \implies n = 1$$

*   **Case 2:** $2^n = \frac{1}{2}$
    $$2^n = 2^{-1} \implies n = -1$$

#### Final Solution Set
Both calculated values are integers, fully satisfying the constraints of the problem statement. The complete integer solution set is:
$$\mathbf{n \in \{-1, 1\}}$$
