# Day 7: Hatsune Miku Video Tasks Challenge

My friend wants to start her own business creating Hatsune Miku videos. She's going to offer discounts to her friends to get things off the ground.

## Challenge Description

Write a function which accepts a 2D array representing video tasks, where the sub-arrays are: `[hour, source]`, an integer `hour` representing how many hours a video takes, and a string `source` representing where the request for this video came from. Given the following constraints, return an integer representing the amount of money my friend will make after delivering all of the videos in the array.

- If the video comes from a **Close Friend**, she'll charge $25 an hour
- If the video comes from a **Friend**, she'll charge $50 an hour
- If the video comes from an **Acquaintance**, she'll charge $100 an hour
- Otherwise, she'll charge $125 an hour

Note that she's lazy and might type the source in all lowercase, or all uppercase - be sure to account for that in your logic.

## Test Cases

1. `[[10, 'Close Friend'], [3, 'Acquaintance'], [7, 'Lead from web'], [6, 'Friend'], [2, 'It came from Facebook']]` should return `1975`
2. `[[2, 'Yahoo'], [50, 'Close friend'], [1, 'Miniworkers'], [4, 'Online Platform'], [6, 'acquaintance']]` should return `2725`
3. `[[1, 'friend'], [8, 'Contact Form'], [3, 'acquaintance'], [4, 'close Friend'], [20, 'Big Job']]` should return `3950`
4. `[]` should return `0`

## 📝 Hints to Solve the Challenge

1. **Normalize Input**:
   - Convert the source string to lowercase to handle different capitalizations.
   
2. **Charge Calculation**:
   - Use a dictionary to map sources to their respective hourly charges.
   
3. **Iterate Through Tasks**:
   - Loop through each task, lookup the charge rate from the dictionary, and calculate the total earnings.
   
## Example Walkthrough

1. **Example Input**: `[[10, 'Close Friend'], [3, 'Acquaintance'], [7, 'Lead from web'], [6, 'Friend'], [2, 'It came from Facebook']]`
   - **Step-by-Step**:
     - `10 hours` from a `Close Friend` at `$25/hour` = `$250`
     - `3 hours` from an `Acquaintance` at `$100/hour` = `$300`
     - `7 hours` from `Lead from web` at `$125/hour` = `$875`
     - `6 hours` from a `Friend` at `$50/hour` = `$300`
     - `2 hours` from `It came from Facebook` at `$125/hour` = `$250`
   - **Result**: Total earnings = `$1975`

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day6/day6.md)** | **[Next Challenge](../../day%20logs/day8/day8.md)** ➡️

---
