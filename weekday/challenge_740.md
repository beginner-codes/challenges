# Challenge 740 - Simple Row Sum

Imagine this triangle:
```python
    1
   2 3
  4 5 6
 7 8 9 10
...
```
Create a function that takes a number `n` and returns the sum of all numbers in the nth row.

## Examples
```python
row_sum(1) ➞ 1

row_sum(2) ➞ 5

row_sum(4) ➞ 34
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


def row_sum(n: int) -> int:
    return 0  # Put your code here!!!


test(740, row_sum)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
  {
    "args": [
      158
    ],
    "return": 1972235
  },
  {
    "args": [
      785
    ],
    "return": 241868705
  },
  {
    "args": [
      445
    ],
    "return": 44060785
  },
  {
    "args": [
      940
    ],
    "return": 415292470
  },
  {
    "args": [
      274
    ],
    "return": 10285549
  }
]
```

## Credits

Found on Edabit: [Simple Row Sum](https://edabit.com/challenge/ysgbRFTPujx8v37yF)
