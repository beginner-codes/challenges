# Challenge 670 - Find Number of Repetitions of Substring

Create a function that takes a string as an argument and tells the number of repetitions of a substring. It is exactly the opposite to repeating a string function (i.e. if a string `k` is given make a larger string `z` such that `k` is repeated `n` times).

In this scenario, we do the opposite. Given the final string, find the number of times the substring is repeated.

## Examples
```python
number_of_repetitions("abcabcabcabc" ) ➞ 4

number_of_repetitions("bcbcbc") ➞ 3

number_of_repetitions("llbllbllbllbllbllb") ➞ 6

number_of_repetitions("kc") ➞ 1
```
## Notes

- Assume that the substring length is always greater than 1.
- Assume that the string length is always greater than 1.
- Assume that the substring is not always the same.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def number_of_repetitions(string: str) -> int:
    return 0  # Put your code here!!!


test(670, number_of_repetitions)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "abc"
        ],
        "return": 1
    },
    {
        "args": [
            "LVLVLVLV"
        ],
        "return": 4
    },
    {
        "args": [
            "abcabcabc"
        ],
        "return": 3
    },
    {
        "args": [
            "aabaab"
        ],
        "return": 2
    },
    {
        "args": [
            "inkinkinkinkinkink"
        ],
        "return": 6
    }
]
```
## Credits

Found on Edabit: [Find Number of Repetitions of Substring](https://edabit.com/challenge/wNMyGvSuBucrvHrmC)
