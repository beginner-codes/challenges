# Challenge 547 - Narcissistic Numbers

A number is narcissistic when the sum of its digits each raised to the power of the number of digits in the number is equal to the number itself.
```python
153 ➞ 3 digits ➞ 1³ + 5³ + 3³ = 1 + 125 + 27 = 153 ➞ Narcissistic
84 ➞ 2 digits ➞ 8² + 4² = 64 + 16 = 80 ➞ Not narcissistic
```
Given a positive integer `n`, implement a function that returns `True` if the number is narcissistic, and `False` if it's not.

## Examples
```javascript
is_narcissistic(8208) ➞ True
// 8⁴ + 2⁴ + 0⁴ + 8⁴ = 8208

is_narcissistic(22) ➞ False
// 2² + 2² = 8

is_narcissistic(9) ➞ True
// 9¹ = 9
```
## Notes

- Trivially, any number in the `1-9` range is narcissistic and any two-digit number is not.
- Curious fact: Only 88 numbers are narcissistic.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def is_narcissistic(number: int) -> bool:
    return False # Put your code here!!!


test(547, is_narcissistic)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            472335975
        ],
        "return": true
    },
    {
        "args": [
            42300981
        ],
        "return": false
    },
    {
        "args": [
            548834
        ],
        "return": true
    },
    {
        "args": [
            886243
        ],
        "return": false
    },
    {
        "args": [
            66
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Narcissistic Numbers](https://edabit.com/challenge/6DwrhEGSa6WDixA5u)
