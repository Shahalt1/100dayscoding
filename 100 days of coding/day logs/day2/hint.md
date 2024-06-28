# Day 2: Go Board Game Winner Calculation - Hint

### Problem Breakdown

1. **Input:** You have a 2D array representing a Go board where each cell can be `"W"`, `"B"`, or `"X"`.
2. **Output:** Determine the winner based on the count of `"W"` (white stones) and `"B"` (black stones).
   - Return `"W:#"` if white has more stones.
   - Return `"B:#"` if black has more stones.
   - Return `"T:#"` if both have the same number of stones.

### Steps to Approach

1. **Initialize Counters:** Start with counters for white (`countW`) and black (`countB`) stones.
2. **Iterate through the Board:** Use nested loops to traverse each element of the 2D array.
   - Increment `countW` for each `"W"`.
   - Increment `countB` for each `"B"`.
3. **Comparison:** After iterating through the board,
   - Compare `countW` and `countB`.
   - Construct the result based on which counter is greater or if they are equal.

### Example Walkthrough

- For a board like:

```
[
    ["W","W","W","B","B","B"],
    ["W","W","W","W","B","B"],
    ["W","W","W","B","B","B"],
    ["W","X","W","B","B","B"],
    ["X","W","B","B","B","B"],
    ["W","W","B","X","B","X"]
]
```

Calculate `countW` and `countB`, then determine the output based on their values.

---

### Navigation

✨ **[Return to Challenge](day2.md)**

---
