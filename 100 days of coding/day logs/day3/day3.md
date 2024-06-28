# Day 3 : Birthday Candle Blowing Challenge

Planning for a birthday party can be a lot of fun, especially when adding unique elements like "trick" candles. These candles require multiple attempts to blow out, and we need to ensure the birthday girl doesn't overexert herself. Let's figure out the total number of attempts needed to blow out all the candles!

## Challenge Description

Write a function that accepts a numerical string, where each digit represents the number of attempts required to blow out the candle at that position. The function should account for the following constraints:

- Blowing out a candle also extinguishes the two candles behind it (the two digits to the right in the string).
- You must blow out the candles from left to right, without skipping any.
- The candles cannot be rearranged.
- Each candle requires between 0 and 9 attempts to be extinguished.
- There will never be more than 12 candles (digits) in the string.

The function should return the total number of attempts required to extinguish all the candles.

### Example

Consider the string `"1321"`. It takes 3 attempts to blow out all the candles:

1. **First attempt:** Blow out the first candle:
   - String changes from `(132)1` to `0211`
2. **Second attempt:** Blow out the next candle:
   - String changes from `0(211)` to `0100`
3. **Third attempt:** Blow out the last candle:
   - String changes from `0(100)` to `0000`

Thus, `"1321"` takes 3 attempts.

### Test Cases

- `"0323456"` should return 9
- `"2113"` should return 5
- `"100100100"` should return 3
- `"102201"` should return 3

Feel free to use any programming language to solve this challenge!

Difficult to solve this challenge, try the following [hints](hint.md)

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day2/day2.md)** | **[Next Challenge](../../day%20logs/day4/day4.md)** ➡️

---
