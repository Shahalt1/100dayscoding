# Day 13: Snail Climbing Challenge

## Challenge Description

Here is your challenge: Write a function `snail` which takes three arguments:
- A number representing the height of the tree.
- A number representing the height the snail can climb each day.
- A number representing the height the snail loses by slipping backwards as it sleeps at night.

The function should return the number of days it will take the snail to reach the top of the tree.

### Test Cases

- `snail(3, 2, 1)` => `2`
- `snail(10, 3, 1)` => `5`
- `snail(10, 3, 2)` => `8`
- `snail(100, 20, 5)` => `7`
- `snail(5, 10, 3)` => `1`

### Explanation

- **snail(3, 2, 1)**:
  - Day 1: Climbs to height 2.
  - Night 1: Slips back to height 1.
  - Day 2: Climbs to the top (height 3).
  - Total Days: 2.

- **snail(10, 3, 1)**:
  - Day 1: Climbs to height 3.
  - Night 1: Slips back to height 2.
  - Day 2: Climbs to height 5.
  - Night 2: Slips back to height 4.
  - Day 3: Climbs to height 7.
  - Night 3: Slips back to height 6.
  - Day 4: Climbs to height 9.
  - Night 4: Slips back to height 8.
  - Day 5: Climbs to the top (height 10).
  - Total Days: 5.

- **snail(5, 10, 3)**:
  - Day 1: Climbs to the top (height 5).
  - Total Days: 1.

You may use any language you'd like to solve this challenge. This is a particularly good one for trying new languages, so don't be afraid to solve it more than once~!

---

### Hints to Solve the Challenge

1. **Initial Climb**:
   - Consider the snail’s net progress each day (climb height - slip height).

2. **Final Climb**:
   - Account for the last day's climb separately if the snail reaches or surpasses the tree height without slipping back.

3. **Edge Cases**:
   - Consider scenarios where the snail reaches the top in one day.
   - Consider the case where the snail’s climb height is greater than the tree height.

---

### Example Walkthrough

#### Example Input
`snail(10, 3, 1)`

#### Step-by-Step Solution

1. Calculate net progress each day:
   - Net progress = 3 - 1 = 2.

2. Determine the days to reach or surpass the height:
   - Remaining height after each day’s climb but before slipping back:
     - Day 1: 3 (remaining 7).
     - Day 2: 5 (remaining 5).
     - Day 3: 7 (remaining 3).
     - Day 4: 9 (remaining 1).
     - Day 5: 10 (reaches the top).

### Result
`5`

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day12/day12.md)** | **[Next Challenge](../../day%20logs/day14/day14.md)** ➡️

---
