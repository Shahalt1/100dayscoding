# Day 4: Card Game War Challenge

I've been into card games lately. A good way to pass the time, if you've heard of it, is War. I've tweaked it a bit after playing a 6-hour match with my sister 😓

## Challenge Description

The premise is simple: the two players each flip a card at the same time. Whomever has the highest value gets the point. If the cards are the same value, neither player gets a point.

### Rules

- The left side of the array represents the top of the deck, and both players flip the top-most card each turn.
- I used to hit the poker tables regularly, so I've got a LOT of card decks floating around my house. This means our decks of cards can be quite massive. BUT the two players' card sets will always be the same size.
- Cards are represented as follows:
  - 10s are represented with `T`
  - Jacks are represented with `J`
  - Queens are represented with `Q`
  - Kings are represented with `K`
  - Aces are represented with `A`
- Card values:
  - Jacks are worth 11
  - Queens are worth 12
  - Kings are worth 13
  - Aces are worth 15

### Challenge

Write a function that takes two arrays of strings: the first representing my set of cards and the second representing my opponent's set of cards. Your function should determine who is going to win based on the rules above.

### Test Cases

1. `['A', '7', '8'], ['K', '5', '9']` should return "Naomi wins 2 to 1"
2. `['T', '9'], ['T', 'A']` should return "Opponent wins 1 to 0"
3. `['2', '3', '4', '5', '6', '7', '8', '9', 'T', 'J', 'Q', 'K', 'A', '5', '6', '8', 'T', '3', 'T', 'J'], ['A', 'K', 'Q', 'J', 'T', '9', '8', '7', '6', '5', '4', '3', '2', '2', '2', 'T', 'T', '9', '4', '3']` should return "Naomi wins 10 to 8"
4. `['A', 'K', '2', '3', 'A', '8', '5', '5', '7', 'T'], ['K', 'A', '5', '9', 'A', '3', '2', '6', '3', 'T']` should return "Tie"

### Hint

1. Map the card characters to their respective values.
2. Iterate through the card arrays, comparing values and keeping score for each player.
3. Determine the winner based on the scores.
4. For more [Hints](hint.md)

You may use any programming language to solve this challenge!

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day3/day3.md)** | **[Next Challenge](../../day%20logs/day5/day5.md)** ➡️

---
