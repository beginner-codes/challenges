# Challenge 449 - Bingo Check

Create a function that takes a 5x5 2D list and returns True if it has at least one Bingo, and False if it doesn't.

## Examples
```python
bingo_check([
  [45, "x", 31, 74, 87],
  [64, "x", 47, 32, 90],
  [37, "x", 68, 83, 54],
  [67, "x", 98, 39, 44],
  [21, "x", 24, 30, 52]
]) ➞ True

bingo_check([
  ["x", 43, 31, 74, 87],
  [64, "x", 47, 32, 90],
  [37, 65, "x", 83, 54],
  [67, 98, 39, "x", 44],
  [21, 59, 24, 30, "x"]
]) ➞ True

bingo_check([
  ["x", "x", "x", "x", "x"],
  [64, 12, 47, 32, 90],
  [37, 16, 68, 83, 54],
  [67, 19, 98, 39, 44],
  [21, 75, 24, 30, 52]
]) ➞ True

bingo_check([
  [45, "x", 31, 74, 87],
  [64, 78, 47, "x", 90],
  [37, "x", 68, 83, 54],
  [67, "x", 98, "x", 44],
  [21, "x", 24, 30, 52]
]) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
  {
    "args": [
      [
        [45, "x", 31, 74, 87],
        [64, "x", 47, 32, 90],
        [37, "x", 68, 83, 54],
        [67, "x", 98, 39, 44],
        [21, "x", 24, 30, 52]
      ]
    ],
    "return": true
  },
  {
    "args": [
      [
        ["x", 43, 31, 74, 87],
        [64, "x", 47, 32, 90],
        [37, 65, "x", 83, 54],
        [67, 98, 39, "x", 44],
        [21, 59, 24, 30, "x"]
      ]
    ],
    "return": true
  },
  {
    "args": [
      [
        [37, 16, 84, 51, 33],
        [64, 12, 47, 32, 90],
        ["x", "x", "x", "x", "x"],
        [67, 19, 98, 39, 44],
        [21, 75, 24, 30, 52]
      ]
    ],
    "return": true
  },
  {
    "args": [
      [
        [45, "x", 31, 74, 87],
        [64, 78, "x", "x", 90],
        [37, "x", 68, "x", 54],
        [67, "x", 98, "x", "x"],
        [21, "x", 24, 30, 52]
      ]
    ],
    "return": false
  },
  {
    "args": [
      [
        [45, 46, 31, 74, "x"],
        [64, 78, 80, "x", 90],
        [37, 81, "x", 55, 54],
        [67, "x", 98, 34, 77],
        ["x", 33, 24, 30, 52]
      ]
    ],
    "return": true
  }
]
```
## Credits

Found on Edabit: [Bingo Check](https://edabit.com/challenge/mJpjpgxkxvTY4Qbwf)
