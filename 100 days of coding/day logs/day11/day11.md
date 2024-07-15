# Day 11: Video Progress Ratio

I'm trying to watch some Youtube tutorials to learn every programming language in the world at the same time. But it's turning into quite the slog. I wanna be able to reward my progress. So I want a quick way to tell if I'm a third of the way through a video, or half way, and such.

## Challenge Description

Here is your challenge: Write a function which accepts two strings in "HH:MM:SS" format - the first string representing how far I've watched the video, and the second representing how long the video is. The function should return an array of two integers, representing the ratio of the video I have watched (e.g. `[1, 3]` if I have made it exactly a third of the way through).

### Test Cases

- `video_part("02:20:00","07:00:00")` => `[1, 3]`
- `video_part("25:26:20","25:26:20")` => `[1, 1]`
- `video_part("00:02:20","00:10:00")` => `[7, 30]`

### Hints to Solve the Challenge

1. **Convert Time to Seconds**:
   - Parse the "HH:MM:SS" format strings to extract hours, minutes, and seconds.
   - Convert the total time into seconds for easier calculations.

2. **Calculate the Greatest Common Divisor (GCD)**:
   - To simplify the ratio, calculate the GCD of the two time values in seconds.
   - Use the GCD to reduce the ratio to its simplest form.

3. **Form the Ratio**:
   - Divide both the watched time and total time by the GCD to get the simplest ratio.

---

### Example Walkthrough

#### Example Input
`video_part("02:20:00","07:00:00")`

#### Step-by-Step Solution

1. Convert both times to seconds:
   - Watched time: \( 2 * 3600 + 20 * 60 + 0 = 8400 \) seconds
   - Total time: \( 7 * 3600 + 0 * 60 + 0 = 25200 \) seconds
   
2. Calculate the GCD of 8400 and 25200:
   - GCD(8400, 25200) = 8400

3. Form the ratio:
   - \([ 8400 / 8400, 25200 / 8400 ] = [1, 3]\)

### Result
`[1, 3]`

---

### Navigation

✨ **[Return to Main README](../../readme.md)**

📚 **[Explore All Challenges](../../challenges1.md)**

⬅️ **[Previous Challenge](../../day%20logs/day10/day10.md)** | **[Next Challenge](../../day%20logs/day12/day12.md)** ➡️

---
