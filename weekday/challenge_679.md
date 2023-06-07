# Challenge 679 - Sum of Round Numbers

Given a number, find the "round" of each digit of the number. An integer is called "round" if all its digits except the leftmost (most significant) are equal to zero.

Round numbers: 4000, 1, 9, 800, 90
Not round numbers: 110, 707, 222, 1001

Create a function that takes a number and returns the "round" of each digit (except if the digit is zero) as a string. Check out the following examples for more clarification.

## Examples
```python
sum_round(101) ➞ "1 100"

sum_round(1234) ➞ "4 30 200 1000"

sum_round(54210) ➞ "10 200 4000 50000"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def sum_round(number: int) -> str:
    return ""  # Put your code here!!!


test(679, sum_round)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            1010
        ],
        "return": "10 1000"
    },
    {
        "args": [
            54213
        ],
        "return": "3 10 200 4000 50000"
    },
    {
        "args": [
            1234
        ],
        "return": "4 30 200 1000"
    },
    {
        "args": [
            548741
        ],
        "return": "1 40 700 8000 40000 500000"
    },
    {
        "args": [
            1234567
        ],
        "return": "7 60 500 4000 30000 200000 1000000"
    }
]
```
## Credits

Found on Edabit: [Sum of Round Numbers](https://edabit.com/challenge/qrSc3vKCqyFcz9ptr)
