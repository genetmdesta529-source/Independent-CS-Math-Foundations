### Mathematical Analysis: Problem A (Sequence Extension & Closed-Forms)

#### Problem Statement
Continue the two sequences of numbers below and find an equation to calculate the $n$-th value:

| $n$ | 1 | 2 | 3 | 4 | 5 | 6 | 7 | Equation |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :--- |
| $a_n$ | 2 | 5 | 10 | 17 | 26 | 37 | ? | ? |
| $b_n$ | 1 | 2 | 8 | 48 | 384 | 3840 | ? | ? |

---

#### 1. Analysis of Sequence $a_n$

**Pattern Recognition:**
Let's analyze the difference between consecutive terms:
*   $a_2 - a_1 = 5 - 2 = 3$
*   $a_3 - a_2 = 10 - 5 = 5$
*   $a_4 - a_3 = 17 - 10 = 7$
*   $a_5 - a_4 = 26 - 17 = 9$

The first differences form a sequence of consecutive odd numbers ($3, 5, 7, 9, 11, \dots$). This indicates a quadratic growth rate related directly to perfect squares:
*   $a_1 = 1^2 + 1 = 2$
*   $a_2 = 2^2 + 1 = 5$
*   $a_3 = 3^2 + 1 = 10$

**Extension for $n=7$:**
$$a_7 = 7^2 + 1 = 49 + 1 = 50$$

**General Equation:**
$$a_n = n^2 + 1$$

---

#### 2. Analysis of Sequence $b_n$

**Pattern Recognition:**
Let's analyze the ratios between consecutive terms:
*   $b_2 / b_1 = 2 / 1 = 2$
*   $b_3 / b_2 = 8 / 2 = 4$
*   $b_4 / b_3 = 48 / 8 = 6$
*   $b_5 / b_4 = 384 / 48 = 8$
*   $b_6 / b_5 = 3840 / 384 = 10$

The multiplier sequence increases by $2$ at each step ($2, 4, 6, 8, 10, \dots$). The recurrence relation is defined as $b_n = b_{n-1} \cdot 2(n-1)$. Expanding this yields:
$$b_n = 1 \cdot 2 \cdot 4 \cdot 6 \dots \cdot 2(n-1)$$
Factoring out a $2$ from each of the $(n-1)$ terms:
$$b_n = 2^{n-1} \cdot [1 \cdot 2 \cdot 3 \dots \cdot (n-1)] = 2^{n-1}(n-1)!$$

**Extension for $n=7$:**
$$b_7 = b_6 \cdot 2(7-1) = 3840 \cdot 12 = 46080$$

**General Equation:**
$$b_n = 2^{n-1}(n-1)! \quad \text{where } 0! = 1$$

---

#### Final Solution Summary
*   **Term $a_7$:** $50$ | **Equation:** $a_n = n^2 + 1$
*   **Term $b_7$:** $46080$ | **Equation:** $b_n = 2^{n-1}(n-1)!$
