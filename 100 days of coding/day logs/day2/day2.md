# Day 2: Go Board Game Winner Calculation

Learning the game of Go can be challenging, but understanding the winner based on stone count doesn't have to be! Here's a function challenge to help you practice:

### Challenge Description

Write a function that takes a 2D array of strings representing a Go board. Each element in the array can be:

- `W` for a white stone
- `B` for a black stone
- `X` for an empty space

Your function should calculate the winner of the
game by counting the number of black stones and white stones. If white has more stones, return `"W:#"` where `#` is the number of white stones. If black has more stones, return `"B:#"` where `#` is the number of black stones. If both have the same number of stones, return `"T:#"` where `#` is the number of stones either player has.

### Examples

- For the board:

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

The function should return `"B:17"`.

- For the board:

```
[
["B", "B", "B", "B", "B", "W", "W", "W", "W"],
["B", "B", "B", "B", "W", "W", "W", "W", "W"],
["B", "B", "B", "W", "W", "W", "W", "W", "W"],
["B", "B", "B", "B", "W", "W", "W", "W", "B"],
["B", "B", "B", "W", "W", "W", "W", "B", "B"],
["B", "B", "W", "W", "W", "W", "B", "B", "B"],
["B", "B", "B", "W", "W", "B", "B", "B", "B"],
["B", "B", "B", "W", "W", "W", "B", "X", "W"],
["B", "B", "B", "B", "B", "W", "B", "W", "W"]
]
```

The function should return `"B:44"`.

---

Feel free to use any programming language of your choice to solve this challenge!

For more details and to participate, visit the [Challenge Repository](https://github.com/Shahalt1/100dayscoding).

Difficult to solve this challenge, try the following [hints](hint.md)

---

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day1/day1.md)** | **[Next Challenge](../../problem)** ➡️

---
