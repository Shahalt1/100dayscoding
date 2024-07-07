# Day 9: Sum of Squares

Let's start the week off with one I hope is not too complex.

## Challenge Description

Here's your challenge: Create a function `squares`. The function should take one argument `n`, which is a positive integer. The function should return the sum of all squared positive integers between 1 and `n`, inclusive.

### Basic Bounds

- 1 ≤ n ≤ 10,000,000

### Advanced Bounds

- 1 ≤ n ≤ 10,000,000,000,000,000,000,000,000

## Test Cases

1. `squares(5)` should return `55`.
2. `squares(10)` should return `385`.
3. `squares(25)` should return `5,525`.
4. `squares(100)` should return `338,350`.

## Hints to Solve the Challenge

1. **Understanding the Sum of Squares Formula**:
   - The sum of squares of the first `n` positive integers can be calculated using the formula:
     \[
     S = \frac{n(n + 1)(2n + 1)}{6}
     \]
     which translates to: S = n * (n + 1) * (2n + 1) / 6.
   - This formula can help in calculating the sum efficiently, even for large values of `n`.

2. **Edge Cases**:
   - Consider the minimum value `n = 1` and ensure your function handles it correctly.
   - For advanced bounds, make sure your function handles very large numbers without running into performance issues.

3. **Optimization Considerations**:
   - For large values of `n`, directly iterating through all numbers and summing their squares might not be feasible. Use the sum of squares formula for efficient computation.

---

### Example Walkthrough

#### Example Input
`squares(5)`

#### Step-by-Step Solution

1. Calculate the sum of squares for `n = 5` using the formula:
   - S = 5 * (5 + 1) * (2 * 5 + 1) / 6
   - S = 5 * 6 * 11 / 6 = 55

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day8/day8.md)** | **[Next Challenge](../../day%20logs/day10/day10.md)** ➡️

---
