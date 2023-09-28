# Challenge 760 - Look and Say Numbers

Given an integer, return a new integer according to the rules below:

- Split the number into groups of two-digit numbers. If the number has an odd number of digits, return `"invalid"`.
- For each group of two-digit numbers, concatenate the last digit to a new string the same number of times as the value of the first digit.

Return the result as an integer.

```python
look_and_say(3132) ➞ 111222

# By reading the number digit by digit, you get three "1" and three "2".
# Therefore, you put three ones and three two's together.
# Remember to return an integer.
```
## Examples
```python
look_and_say(95) ➞ 555555555

look_and_say(1213141516171819) ➞ 23456789

look_and_say(120520) ➞ 200

look_and_say(231) ➞ "invalid"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def look_and_say(number: int) -> int:
    return 0  # Put your code here!!!


test(760, look_and_say)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            830756
        ],
        "return": 3333333366666
    },
    {
        "args": [
            1213141516171819
        ],
        "return": 23456789
    },
    {
        "args": [
            75282
        ],
        "return": "invalid"
    },
    {
        "args": [
            488280
        ],
        "return": 88882222222200000000
    },
    {
        "args": [
            890917
        ],
        "return": 999999997
    }
]
```

## Credits

Found on Edabit: [Look and Say Numbers](https://edabit.com/challenge/6hnrKRh7fZfMC5CKY)
