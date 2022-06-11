# Challenge 475 - English to Numbers

Given an English description of an integer in the range `0` to `999`, devise a function that returns the integer in numeric form.

## Examples
```python
eng2nums("four") ➞  4

eng2nums("forty") ➞ 40

eng2nums("six hundred") ➞ 600

eng2nums("one hundred fifteen") ➞ 115

eng2nums("seven hundred sixty seven") ➞ 767
```
## Notes

- No hyphens are used in test cases ("twenty three" not "twenty-three").
- The word "and" is not used: "one hundred three" not "one hundred and three".

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def eng2num(number: str) -> int:
    return 0  # Put your code here!!!


test(475, eng2num)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "one"
        ],
        "return": 1
    },
    {
        "args": [
            "ninety"
        ],
        "return": 90
    },
    {
        "args": [
            "one hundred ten"
        ],
        "return": 110
    },
    {
        "args": [
            "sixty two"
        ],
        "return": 62
    },
    {
        "args": [
            "four hundred thirty"
        ],
        "return": 430
    },
    {
        "args": [
            "zero"
        ],
        "return": 0
    },
    {
        "args": [
            "four hundred fifty six"
        ],
        "return": 456
    },
    {
        "args": [
            "six hundred nine"
        ],
        "return": 609
    },
    {
        "args": [
            "seven hundred"
        ],
        "return": 700
    },
    {
        "args": [
            "thirty seven"
        ],
        "return": 37
    },
    {
        "args": [
            "nine hundred ninety nine"
        ],
        "return": 999
    },
    {
        "args": [
            "three hundred twelve"
        ],
        "return": 312
    },
    {
        "args": [
            "eighteen"
        ],
        "return": 18
    },
    {
        "args": [
            "five hundred eleven"
        ],
        "return": 511
    }
]
```
## Credits

Found on Edabit: [English to Numbers](https://edabit.com/challenge/9cuQrhEMwiESfKznk)
