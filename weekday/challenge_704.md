# Challenge 704 - Kaprekar Numbers

A Kaprekar Number is a positive integer that is equal to a number formed by first squaring, then splitting and summing its two lexicographical parts:

- If the quantity of digits of the squared number is even, the left and right parts will have the same length.
- If the quantity of digits of the squared number is odd, then the right part will be the longer half, with the left part being the shorter or equal to zero if the quantity of digits is equal to 1.

Given a positive integer implement a function that returns `True` if it's a Kaprekar number, and `False` if it's not.

## Examples
```python
is_kaprekar(3) ➞ False
# n² = "9"
# Left + Right = 0 + 9 = 9 ➞ 9 != 3

is_kaprekar(5) ➞ False
# n² = "25"
# Left + Right = 2 + 5 = 7 ➞ 7 != 5

is_kaprekar(297) ➞ True
# n² = "88209"
# Left + Right = 88 + 209 = 297 ➞ 297 == 297
```
## Notes

- Trivially, 0 and 1 are Kaprekar Numbers being the only two numbers equal to their square.
- Any number formed only by digits equal to 9 will always be a Kaprekar Number.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def is_kaprekar(number: int) -> bool:
    return False  # Put your code here!!!


test(704, is_kaprekar)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            1
        ],
        "return": true
    },
    {
        "args": [
            1441
        ],
        "return": false
    },
    {
        "args": [
            102102
        ],
        "return": false
    },
    {
        "args": [
            9
        ],
        "return": true
    },
    {
        "args": [
            77778
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Kaprekar Numbers](https://edabit.com/challenge/GX3pQxvbTJApWYgRJ)
