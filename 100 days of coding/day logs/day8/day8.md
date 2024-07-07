# Day 8: Gradient Colour Calculation for Discord Embeds

I had a client that wanted a series of Discord embeds generated. Part of the spec was that the embeds needed to have a gradient colour - that is, scrolling through them shows the colour on the side gradually changing from green to blue. The other caveat was that the number of embeds being generated was variable, so I could not hard code the colours. And what do you do when you have a variable amount of data? Make a function!

## Challenge Description

Create a function that takes an integer `index`, and an integer `max`. The `index` will represent the current "step" you are along the gradient scale, and the `max` will represent the total number of steps.

The function should then calculate from a "start" hex and an "end" hex, using the `index` and `max`, to determine the correct hex code for this step along the gradient. The value returned should be a hexadecimal number.

### Requirements

1. The calculation needs to work for both circumstances: When start is a higher value than end, and when start is a lower value than end.
2. There are minimum and maximum bounds you will need to set for your calculations.

### Hint

You will need to split `start` and `end` into segments for each colour value (hex codes are `RRGGBB`). Life will be easier if these are strings.

**I had to get help with this one myself. So I encourage you all to collaborate and have fun with it! You are free to use any language you like.**

**Bonus points if you make `start` and `end` parameters instead of hardcoding them.**

## Test Cases

1. `gradientColor(0, 10, "00FF00", "0000FF")` should return `#00FF00` (start color)
2. `gradientColor(5, 10, "00FF00", "0000FF")` should return `#007F80` (midpoint color)
3. `gradientColor(10, 10, "00FF00", "0000FF")` should return `#0000FF` (end color)
4. `gradientColor(2, 5, "FF0000", "00FF00")` should return `#80BF00` (second step)
5. `gradientColor(5, 5, "FF0000", "00FF00")` should return `#00FF00` (end color)
6. `gradientColor(3, 7, "FFFFFF", "000000")` should return `#555555` (almost halfway)

## 📝 Hints to Solve the Challenge

1. **Color Splitting**:
   - Convert the start and end colors from hex to RGB.
   - Split the hex codes into their R, G, and B components.

2. **Interpolation Calculation**:
   - For each color component, calculate the interpolated value using the formula:
     - `R = startR + (endR - startR) * (index / max)`
     - `G = startG + (endG - startG) * (index / max)`
     - `B = startB + (endB - startB) * (index / max)`
   - Ensure the values are rounded to the nearest integer and remain within the bounds of 0 to 255.

3. **Reconstruct Hex Code**:
   - Combine the interpolated RGB values back into a hex code.

## Example Walkthrough

### Example Input
`gradientColor(5, 10, "00FF00", "0000FF")`

### Step-by-Step Solution
1. Convert `start` (`00FF00`) and `end` (`0000FF`) to RGB:
   - `start` = (0, 255, 0)
   - `end` = (0, 0, 255)

2. Calculate the interpolated values for R, G, and B:
   - `R = 0 + (0 - 0) * (5 / 10) = 0`
   - `G = 255 + (0 - 255) * (5 / 10) = 127.5 ≈ 128`
   - `B = 0 + (255 - 0) * (5 / 10) = 127.5 ≈ 128`

3. Combine the interpolated values into a hex code:
   - Interpolated RGB: (0, 128, 128)
   - Hex code: `#007F80`

### Result
`#007F80`

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day7/day7.md)** | **[Next Challenge](../../day%20logs/day9/day9.md)** ➡️

---
