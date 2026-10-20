### Mathematical Analysis: Problem A (Sequence Closed-Form Solution)

#### Problem Statement
A sequence is defined by $a_1 = 1$ and $a_{n+1} = a_n + n + 1$. Find a closed-form equation to calculate the value of $a_n$ and determine $a_{100}$.

#### Step-by-Step Mathematical Derivation

**1. Analyzing the Sequence Behavior:**
Let's compute the first few terms of the sequence to identify a pattern:
*   $a_1 = 1$
*   $a_2 = a_1 + 1 + 1 = 1 + 2 = 3$
*   $a_3 = a_2 + 2 + 1 = 3 + 3 = 6$
*   $a_4 = a_3 + 3 + 1 = 6 + 4 = 10$

The sequence generated ($1, 3, 6, 10, \dots$) represents the classic **triangular numbers**.

**2. Finding the Recurrence Relation Summation:**
We can rewrite the recurrence relation as:
$$a_{n+1} - a_n = n + 1$$

Expressing $a_n$ as a telescoping series sum from the base case $a_1$:
$$a_n = a_1 + \sum_{i=1}^{n-1} (i + 1)$$
$$a_n = 1 + (2 + 3 + 4 + \dots + n)$$

Notice that $1 + 2 + 3 + \dots + n$ is the sum of the first $n$ positive integers. Therefore:
$$a_n = \sum_{i=1}^{n} i$$

Using the standard arithmetic series summation formula:
$$a_n = \frac{n(n + 1)}{2}$$

#### 3. Computing the Value of $a_{100}$
Substitute $n = 100$ into our verified closed-form equation:
$$a_{100} = \frac{100 \times (100 + 1)}{2}$$
$$a_{100} = 50 \times 101 = 5050$$

#### Final Solutions
*   **Closed-form Equation:** $\mathbf{a_n = \frac{n(n + 1)}{2}}$
*   **100th Term Value:** $\mathbf{a_{100} = 5050}$
