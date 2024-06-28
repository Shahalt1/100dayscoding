# Day 3: Birthday Candle Blowing Challenge - Hints

## Hints to Solve the Challenge

1. **Understand the Problem**:

   - Each digit in the string represents attempts needed to blow out that candle.
   - Blowing out a candle also affects the two candles behind it.

2. **Approach**:

   - Start from the leftmost candle and move to the right.
   - Track the total attempts required.

3. **Steps**:

   - Initialize a counter for the total attempts.
   - Iterate through the string:
     - For each candle, add its value to the total attempts.
     - Update the attempts needed for the next two candles (set them to zero).
   - Continue until all candles are extinguished.

4. **Example Walkthrough**:
   - For `"1321"`, the steps are:
     1. First attempt on `"1"`: Resulting string `0211`.
     2. Second attempt on `"2"`: Resulting string `0100`.
     3. Third attempt on `"1"`: Resulting string `0000`.
   - Total attempts: 3.

## Test Your Solution

- Use the provided test cases to verify your solution:
  - `"0323456"` should return 9
  - `"2113"` should return 5
  - `"100100100"` should return 3
  - `"102201"` should return 3

---

### Navigation

✨ **[Return to Challenge](day3.md)**

---
