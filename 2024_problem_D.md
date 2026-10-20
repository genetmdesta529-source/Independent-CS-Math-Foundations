### Formal Proof: Problem D (Fermat's Little Theorem & Divisibility)

#### Problem Statement
Prove that $n^5 - n$ is divisible by $5$ for all positive integers $n$.

---

#### Proof Method 1: Algebraic Factorization

**1. Factoring the Polynomial Expression:**
We can break down the expression $n^5 - n$ into smaller linear and quadratic factors:
$$n^5 - n = n(n^4 - 1)$$

Applying the difference of squares identity ($x^2 - y^2 = (x-y)(x+y)$) to $(n^4 - 1)$:
$$n^5 - n = n(n^2 - 1)(n^2 + 1)$$
$$n^5 - n = n(n - 1)(n + 1)(n^2 + 1)$$

**2. Rearranging the Factors:**
Let's rearrange the linear terms in ascending order:
$$(n - 1) \cdot n \cdot (n + 1) \cdot (n^2 + 1)$$

Notice that $(n - 1) \cdot n \cdot (n + 1)$ represents the product of **three consecutive integers**. 

**3. Case-by-Case Divisibility Analysis modulo 5:**
Every integer $n$ can be expressed in one of five forms depending on its remainder when divided by 5 ($n \equiv r \pmod 5$):

*   **Case 1 ($n \equiv 0 \pmod 5$):** The factor $n$ is a multiple of 5, making the entire product a multiple of 5.
*   **Case 2 ($n \equiv 1 \pmod 5$):** The factor $(n - 1) \equiv 0 \pmod 5$, making the entire product a multiple of 5.
*   **Case 3 ($n \equiv 4 \equiv -1 \pmod 5$):** The factor $(n + 1) \equiv 0 \pmod 5$, making the entire product a multiple of 5.
*   **Case 4 ($n \equiv 2 \pmod 5$):** Looking at the quadratic factor:
    $$n^2 + 1 \equiv 2^2 + 1 = 5 \equiv 0 \pmod 5$$
    Thus, $(n^2 + 1)$ is a multiple of 5.
*   **Case 5 ($n \equiv 3 \equiv -2 \pmod 5$):** Looking at the quadratic factor:
    $$n^2 + 1 \equiv (-2)^2 + 1 = 5 \equiv 0 \pmod 5$$
    Thus, $(n^2 + 1)$ is a multiple of 5.

Since every possible integer state leaves at least one factor divisible by 5, the entire expression $n^5 - n$ is perfectly divisible by 5 for all positive integers $n$. $\blacksquare$

---

#### Proof Method 2: Fermat's Little Theorem (High-Level Framework)

Fermat's Little Theorem explicitly states that if $p$ is a prime number, then for any integer $n$:
$$n^p \equiv n \pmod p$$

By substituting the prime value $p = 5$ into the theorem:
$$n^5 \equiv n \pmod 5$$

Subtracting $n$ from both sides yields the final congruence relation directly:
$$n^5 - n \equiv 0 \pmod 5$$

This confirms that $n^5 - n$ is a clean multiple of 5 for any positive integer $n$. $\blacksquare$
