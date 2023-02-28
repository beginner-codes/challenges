# Challenge 614 - Persistent Little Bugger

Create a function that takes an integer and returns its multiplicative persistence, which is the number of times you must multiply the digits in the number until you reach a single digit.

## Examples
```python
bugger(39) ➞ 3
# Because 3 * 9 = 27, 2 * 7 = 14, 1 * 4 = 4 and 4 has only one digit.

bugger(999) ➞ 4
# Because 9 * 9 * 9 = 729, 7 * 2 * 9 = 126, 1 * 2 * 6 = 12, and finally 1 * 2 = 2.

bugger(4) ➞ 0
# Because 4 is already a one-digit number.
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def bugger(number: int) -> int:
    return 0  # Put your code here!!!


test(614, bugger)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            999
        ],
        "return": 4
    },
    {
        "args": [
            25
        ],
        "return": 2
    },
    {
        "args": [
            4
        ],
        "return": 0
    },
    {
        "args": [
            39
        ],
        "return": 3
    }
]
```
## Credits

Found on Edabit: [Persistent Little Bugger](https://edabit.com/challenge/yYE8bJ5jhJgAoc5ir)
