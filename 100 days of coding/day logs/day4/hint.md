# Day 4: Card Game War Challenge - Hints

## 📝 Hints to Solve the Challenge

1. **🃏 Understand Card Values**:

   - Create a dictionary to map card characters to their respective values:
     - `2-9` are worth their face values.
     - `T` is worth 10.
     - `J` is worth 11.
     - `Q` is worth 12.
     - `K` is worth 13.
     - `A` is worth 15.

2. **🔄 Iterate Through Cards**:

   - Use a loop to iterate through both players' card arrays simultaneously.
   - For each iteration, compare the values of the corresponding cards.

3. **📊 Keep Score**:

   - Initialize two counters, one for each player (e.g., `naomi_score` and `opponent_score`).
   - For each card comparison:
     - Increment the score of the player with the higher card value.
     - If the card values are the same, no score is awarded.

4. **🏆 Determine the Winner**:
   - After iterating through all the cards, compare the final scores.
   - Return the result in the format: `"Naomi wins X to Y"`, `"Opponent wins X to Y"`, or `"Tie"`.

## 🧪 Example Walkthrough

1. **Example Input**: `['A', '7', '8']`, `['K', '5', '9']`
   - **Step-by-Step**:
     - Compare `A` (15) with `K` (13): Naomi wins this round.
     - Compare `7` (7) with `5` (5): Naomi wins this round.
     - Compare `8` (8) with `9` (9): Opponent wins this round.
   - **Result**: Naomi wins 2 to 1.

## 🔍 Additional Test Cases

- `['T', '9'], ['T', 'A']` should return "Opponent wins 1 to 0"
- `['2', '3', '4', '5', '6', '7', '8', '9', 'T', 'J', 'Q', 'K', 'A', '5', '6', '8', 'T', '3', 'T', 'J'], ['A', 'K', 'Q', 'J', 'T', '9', '8', '7', '6', '5', '4', '3', '2', '2', '2', 'T', 'T', '9', '4', '3']` should return "Naomi wins 10 to 8"
- `['A', 'K', '2', '3', 'A', '8', '5', '5', '7', 'T'], ['K', 'A', '5', '9', 'A', '3', '2', '6', '3', 'T']` should return "Tie"

---

### Navigation

✨ **[Return to Challenge](day4.md)**

---
