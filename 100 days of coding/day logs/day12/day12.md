# Day 12: String Overlap Challenge

So I'm trying to print a bunch of stuff, but printer ink is painfully expensive. I wanna combine things as much as possible. Can you help with that?

## Challenge Description

Here is your challenge: Write a function which takes two string arguments. The function should combine the strings using the largest overlap they share - the ending of the first string should overlap the beginning of the second.

### Examples

- `"abcde" + "cdefgh"` => `"abcdefgh"`
- `"abaab" + "aabab"` => `"abaabab"`
- `"abc" + "def"` => `"abcdef"`
- `"abc" + "abc"` => `"abc"`

The longest overlap means that `"abaabaab" + "aabaabab"` would be `"abaabaabab"` and not `"abaabaabaabab"`.

### Constraints

- The function should find the largest possible overlap.
- Overlap means that the end of the first string should match the beginning of the second string.

You may use any language you'd like to solve this challenge~!

---

### Hints to Solve the Challenge

1. **Identify Overlap**:
   - Iterate through the end of the first string and the beginning of the second string to find the longest match.

2. **Combine Strings**:
   - Once the longest overlap is identified, concatenate the two strings, ensuring the overlap is only counted once.

3. **Edge Cases**:
   - Consider scenarios where there is no overlap at all.
   - Consider scenarios where one string is completely contained within the other.

---

### Example Walkthrough

#### Example Input
`combine_strings("abcde", "cdefgh")`

#### Step-by-Step Solution

1. Identify the longest overlap between the end of the first string and the start of the second string:
   - Overlap: `"cde"`

2. Combine the strings:
   - Result: `"abcdefgh"`

### Result
`"abcdefgh"`

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day11/day11.md)** | **[Next Challenge](../../day%20logs/day13/day13.md)** ➡️

---
