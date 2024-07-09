# Day 10: Clothing Size Conversion

I'm trying to buy some new clothes, but these sizes are so confusing! Maybe you can help?

## Challenge Description

Here is your challenge: Write a function which accepts a string representing a size like "s" or "l", and returns a numerical value for that size given these constraints:

- "s" is equivalent to 36
- "m" is equivalent to 38
- "l" is equivalent to 40

Appending an "x" before "s" decrements the value by 2. Multiple "x"s can be appended in this way.

Appending an "x" before "l" increments the value by 2. Multiple "x"s can be appended in this way.

If the size given to your function does not follow these constraints, return `null`, `None`, or the equivalent in your language.

### Test Cases

- `xs` -> `34`
- `xl` -> `42`
- `xxxs` -> `30`
- `xxxl` -> `46`
- `xm` -> `null`
- `naomi` -> `null`
- `sm` -> `null`
- `lx` -> `null`

## Hints to Solve the Challenge

1. **Parsing the Input**:
   - Determine the base size by checking the last character of the input string.
   - Count the number of "x"s preceding the base size character.

2. **Calculating the Size**:
   - Initialize a base value depending on whether the size is "s", "m", or "l".
   - Adjust the base value based on the number of "x"s found.
   - Ensure to return `null` if the input is invalid (e.g., contains characters other than "x", "s", "m", or "l").

3. **Edge Cases**:
   - Handle edge cases where the input does not match the expected patterns.
   - Ensure the function returns the appropriate value for valid inputs and `null` for invalid ones.

---

### Example Walkthrough

#### Example Input
`squares("xxs")`

#### Step-by-Step Solution

1. Determine the base size:
   - The last character is "s", which has a base value of 36.
   
2. Count the number of "x"s:
   - There are 2 "x"s before "s".
   
3. Calculate the adjusted size:
   - Base value for "s" is 36.
   - Subtract 2 for each "x": 36 - 2 * 2 = 32.

### Result
`32`

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day9/day9.md)** | **[Next Challenge](../../day%20logs/day11/day11.md)** ➡️

---
