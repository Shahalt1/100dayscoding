# Day 6: Creating a Range Function in JavaScript

I don't know about y'all, but I really wish JavaScript had a proper range function. So.... Let's make one! 🎉

## Challenge Description

Write a function `range` which:

1. **Single Parameter**: 
   - Accepts one number, representing the (inclusive) end of the range, and returns an array of numbers from 1 to that end.
   - Example: `range(5)` => `[1, 2, 3, 4, 5]`

2. **Two Parameters**: 
   - Accepts two numbers, representing the start and inclusive end of the range, and returns an array of numbers from start to end.
   - Example: `range(3, 7)` => `[3, 4, 5, 6, 7]`

3. **Three Parameters**: 
   - Accepts three numbers, representing the start, step, and inclusive end of the range, and returns an array of numbers from start to end counting up by step.
   - Example: `range(2, 3, 15)` => `[2, 5, 8, 11, 14]`

In true JavaScript fashion, if someone passes invalid inputs (like a negative number, or a letter), we don't need to worry about that. They should read the ECMAScript spec for our function, that's on them. 🤷 But if you'd like the extra challenge, write your function to account for that:

- Example: `range(-1, 5)` => `[-1, 0, 1, 2, 3, 4, 5]`
- Example: `range(200, 5, "three hundred")` => `TypeError: Arguments must be integers`

And of course, counting down is WAY HARDER and I'm not smart enough for that 😅 But if you are, and you'd like to implement that too, go for it:

- Example: `range(10, 1)` => `[10, 9, 8, 7, 6, 5, 4, 3, 2, 1]`
- Example: `range(10, 3, 3)` => `[10, 7, 4]`

You can use a language other than JavaScript to write this~! But if you do something like use Python's built-in range function, you're kinda just robbing yourself of the joy of solving this! 😜

## Test Cases

1. `range(5)` should return `[1, 2, 3, 4, 5]`
2. `range(3, 7)` should return `[3, 4, 5, 6, 7]`
3. `range(2, 3, 15)` should return `[2, 5, 8, 11, 14]`
4. `range(-1, 5)` should return `[-1, 0, 1, 2, 3, 4, 5]`
5. `range(200, 5, "three hundred")` should return `TypeError: Arguments must be integers`
6. `range(10, 1)` should return `[10, 9, 8, 7, 6, 5, 4, 3, 2, 1]`
7. `range(10, 3, 3)` should return `[10, 7, 4]`

## 📝 Hints to Solve the Challenge

1. **Basic Range**:
   - If the function is called with a single parameter, create an array from 1 to that number.

2. **Start and End Range**:
   - If the function is called with two parameters, create an array from the start number to the end number.

3. **Step Range**:
   - If the function is called with three parameters, create an array starting at the first number, incrementing by the second number, until you reach or exceed the end number.

4. **Edge Cases**:
   - Handle cases where the input is not a valid number.
   - Implement the functionality to count down if the start number is greater than the end number.

## 🧪 Example Walkthrough

1. **Example Input**: `range(5)`
   - **Step-by-Step**:
     - Generate an array from 1 to 5.
   - **Result**: `[1, 2, 3, 4, 5]`

2. **Example Input**: `range(3, 7)`
   - **Step-by-Step**:
     - Generate an array from 3 to 7.
   - **Result**: `[3, 4, 5, 6, 7]`

3. **Example Input**: `range(2, 3, 15)`
   - **Step-by-Step**:
     - Generate an array from 2 to 15, stepping by 3.
   - **Result**: `[2, 5, 8, 11, 14]`

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day5/day5.md)** | **[Next Challenge](../../day%20logs/day7/day7.md)** ➡️

---
