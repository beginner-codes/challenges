# Challenge 445 - Smallest N Digit Number

Write a function that returns the smallest N-digit number which is a multiple of the specified value.

## Examples
```python
smallest(3, 8) ➞ 104
# Smallest 3-digit integer that is a multiple of 8

smallest(5, 12) ➞ 10008

smallest(7, 1) ➞ 1000000

smallest(2, 3) ➞ 12
```
## Notes

- The first arg will be `n` while the second digit will be the specified multiple.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
  {
    "args": [3, 8],
    "return": 104
  },
  {
    "args": [5, 12],
    "return": 10008
  },
  {
    "args": [7, 1],
    "return": 1000000
  },
  {
    "args": [2, 3],
    "return": 12
  },
  {
    "args": [9, 33],
    "return": 100000032
  }
]
```
## Credits

Found on Edabit: [Smallest N Digit Number](https://edabit.com/challenge/WBNgokx2TJTq2aD2N)
