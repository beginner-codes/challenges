# Challenge 754 - Perfect or Amicable?

Given a positive number, if all the positive divisors of that number, excluding the number itself, add up to the number, then it is said to be a perfect number.

For example, the set of positive divisors of 6 excluding 6 itself is 1, 2, and 3. Their sum is 6. Therefore, 6 is a perfect number.

Given a positive number, if all the positive divisors of that number add up to a second number, and all the positive divisors of that add up to the first number, then those two numbers are said to be a pair of amicable numbers.

Create a function that takes a number and returns `"Perfect"` if the number is perfect, `"Amicable"` if the number is part of an amicable pair, or `"Neither"`.

## Examples
```python
num_type(6) ➞ "Perfect"

num_type(2924) ➞ "Amicable"

num_type(5010) ➞ "Neither"
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


def num_type(number: int) -> str:
    return ""  # Put your code here!!!


test(754, num_type)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            2924
        ],
        "return": "Amicable"
    },
    {
        "args": [
            5566
        ],
        "return": "Neither"
    },
    {
        "args": [
            5010
        ],
        "return": "Neither"
    },
    {
        "args": [
            8128
        ],
        "return": "Perfect"
    },
    {
        "args": [
            10744
        ],
        "return": "Amicable"
    }
]
```

## Credits

Found on Edabit: [Perfect or Amicable?](https://edabit.com/challenge/9cNxcMjfEMzKYoBZY)
