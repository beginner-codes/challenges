# Challenge 468 - Converting One Binary String to Another

Write a function that returns the minimum number of swaps to convert the first binary string into the second.

## Examples
```python
min_swaps("1100", "1001") ➞ 1

min_swaps("110011", "010111") ➞ 1

min_swaps("10011001", "01100110") ➞ 4
```
## Notes

- Both binary strings will be of equal length.
- Both binary strings will have an equal number of zeroes and ones.
- A swap is switching two elements in a string (swaps do not have to be adjacent).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def min_swaps(binary_1: str, binary_2: str) -> int:
    return 0  # Put your code here!!!


test(468, min_swaps)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "1001",
            "1001"
        ],
        "return": 0
    },
    {
        "args": [
            "1100",
            "1001"
        ],
        "return": 1
    },
    {
        "args": [
            "110011",
            "010111"
        ],
        "return": 1
    },
    {
        "args": [
            "1100",
            "0011"
        ],
        "return": 2
    },
    {
        "args": [
            "110011",
            "001111"
        ],
        "return": 2
    }
]
```
## Credits

Found on Edabit: [Converting One Binary String to Another](https://edabit.com/challenge/AjZBGWyPaA7rXFhi6)
