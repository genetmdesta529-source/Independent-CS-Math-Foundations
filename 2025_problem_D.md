### Formal Proof: Problem D (Sophie Germain's Identity & Primality)

#### Problem Statement
Prove that for every positive integer $n$, the number $n^4 + 4$ is a composite number, except for one value of $n$.

#### Proof via Polynomial Factorization

**1. Algebraic Factoring (Sophie Germain's Identity):**
To analyze the factorization properties of the expression $n^4 + 4$, we can complete the square by adding and subtracting an intermediate term, $4n^2$:
$$n^4 + 4 = n^4 + 4n^2 + 4 - 4n^2$$

Group the first three terms into a perfect square trinomial:
$$n^4 + 4 = (n^2 + 2)^2 - (2n)^2$$

**2. Difference of Squares Expansion:**
Applying the algebraic identity $x^2 - y^2 = (x - y)(x + y)$, where $x = n^2 + 2$ and $y = 2n$:
$$n^4 + 4 = (n^2 + 2 - 2n)(n^2 + 2 + 2n)$$

Rearranging into standard quadratic form:
$$n^4 + 4 = (n^2 - 2n + 2)(n^2 + 2n + 2)$$

**3. Factoring Evaluation over Positive Integers:**
For $n^4 + 4$ to be a prime number rather than a composite number, the smaller of the two factors must equal $1$. Since $n$ is a positive integer ($n \geq 1$), we evaluate the bounds of both factors:

*   **Factor 1 ($n^2 + 2n + 2$):** Since $n \geq 1$, it is clear that $n^2 + 2n + 2 \geq 1 + 2 + 2 = 5$. Thus, this factor is strictly greater than $1$.
*   **Factor 2 ($n^2 - 2n + 2$):** Let's set this factor equal to $1$ to find our exception case:
    $$n^2 - 2n + 2 = 1$$
    $$n^2 - 2n + 1 = 0$$
    $$(n - 1)^2 = 0 \implies n = 1$$

**4. Testing the Exception Case ($n = 1$):**
If $n = 1$:
$$1^4 + 4 = 5$$
Since $5$ is a prime number, it is not composite. 

**5. Evaluating for all $n > 1$:**
For any integer $n > 1$, the factor $(n^2 - 2n + 2)$ will be strictly greater than $1$. For instance, if $n=2$, the factors are $(2) \times (10) = 20$. Because the expression factors into two distinct integers that are both strictly greater than $1$, the resulting number must be composite.

#### Conclusion
The number $n^4 + 4$ can always be factored into two integers strictly greater than $1$ for all positive integers $n$, making it composite everywhere except when $\mathbf{n = 1}$. $\blacksquare$
