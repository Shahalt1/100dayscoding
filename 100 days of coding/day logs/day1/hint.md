# Day 1: Gacha Character Selection Challenge - Hints

### Understanding the Problem

1. **Input Format:** Each character is represented as an object with properties `name` and `odds`.
2. **Output:** Return the `name` of the character with the highest odds of dropping.

### Steps to Approach

1. **Parse Ratios:** Convert ratio-formatted strings (`X:Y`) into numerical values.
2. **Compare Odds:** Implement a logic to determine which character has the highest odds based on the parsed values.
3. **Iterate Efficiently:** Handle a variable number of input objects without using an array or list structure.

### Implementation Tips

- **String Manipulation:** Use string methods to split and convert ratio strings into integers.
- **Math Operations:** Compare ratios using basic arithmetic operations.
- **Iterative Logic:** Loop through each character object to determine the highest odds.

### Example Walkthrough

- For `{name: "Yinlin", odds: "1:3"}, {name: "Jianxin", odds: "1:2"}`, convert ratios to decimals and compare (`1/3` vs `1/2`).

### Language Flexibility

- Feel free to choose any programming language that best suits your comfort and efficiency in solving this challenge.

---

### Navigation

✨ **[Return to Challenge](day1.md)**

---
