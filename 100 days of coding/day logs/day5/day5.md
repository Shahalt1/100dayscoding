# Day 5: Custom RGB Printer Ink Challenge

I need to print out a bunch of images, but I don't know if I have enough ink! This is a super custom printer that I've got to make my own ink for... Instead of CMYK, it uses RGB ink!

## Challenge Description

Write a function that accepts:

1. A 2D array representing the pixels in the image to print.
2. A 1D array representing the Red, Green, and Blue ink in the printer.

### Constraints

- Each pixel in the image is a 6-digit hexadecimal code.
- The hexadecimal `ffffff` requires 0 Red, 0 Green, and 0 Blue ink.
- The hexadecimal `000000` requires 255 Red, 255 Green, and 255 Blue ink.
- The hexadecimal `fefdfc` requires 1 Red, 2 Green, and 3 Blue ink.

Your function should return `true` if there is enough ink to print the image, and `false` if there is not.

### Test Cases

1. `[['ffffff']], [0, 0, 0]` should return `true` - I don't need ink to print a white page.
2. `[['000000']], [255, 255, 254]` should return `false` - I need one more blue ink.
3. `[['000000', '000000', '000000']], [255, 255, 254]` should return `false` - I have nowhere near enough ink.
4. `[['000000', '000000', '000000']], [768, 768, 768]` should return `true` - I have exactly enough ink.
5. `[['000000']], [400, 526, 612]` should return `true` - I have more than enough ink.
6. `[['fefefe', 'fefefe', 'fefefe'], ['fefefe', 'fefefe', 'fefefe'], ['fefefe', 'fefefe', 'fefefe']], [9, 8, 9]` should return `false` - I need one more unit of green.

---

### Difficult to solve this challenge, try the following [hints](hint.md)

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day4/day4.md)** | **[Next Challenge](../../day%20logs/day6/day6.md)** ➡️

---
