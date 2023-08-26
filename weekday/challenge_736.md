# Challenge 736 - The Complete Bracelet

A complete bracelet is a list with at least one subsequence (pattern) repeating at least two times, and completely - the
subsequence cannot be cut-off at any point. The subsequence must have length two or greater.

Complete bracelets:

```python
[1, 2, 3, 3, 1, 2, 3, 3]  # Pattern: [1, 2, 3, 3]

[1, 2, 1, 2, 1, 2, 1, 2]  # Pattern: [1, 2] or [1, 2, 1, 2]

[1, 1, 6, 1, 1, 7, 1, 1, 6, 1, 1, 7, 1, 1, 6, 1, 1, 7]  # Pattern: [1, 1, 6, 1, 1, 7]

[4, 4, 3, 4, 4, 4, 4, 3, 4, 4]  # Pattern: [4, 4, 3, 4, 4]
```

Incomplete bracelets:

```
[1, 2, 2, 2, 1, 2, 2, 2, 1]  # Incomplete (chopped off)

[1, 1, 6, 1, 1, 7]  # Incomplete (subsequence repeats only once)
```

Create a function that returns `True` if a bracelet is complete, and `False` otherwise.

## Examples

```python
complete_bracelet([1, 2, 2, 1, 2, 2]) ➞ True

complete_bracelet([5, 1, 2, 2]) ➞ False

complete_bracelet([5, 5, 5]) ➞ False
# potential pattern [5, 5] cut-off (patterns >= 2)
```

## Notes

- Patterns must be at least two integers in length.

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


def complete_bracelet(numbers: list[int]) -> bool:
    return False  # Put your code here!!!


test(736, complete_bracelet)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
  {
    "args": [
      [
        5,
        5
      ]
    ],
    "return": false
  },
  {
    "args": [
      [
        5,
        2,
        5,
        5,
        2,
        5,
        2,
        5,
        2,
        2,
        5,
        2,
        5,
        2,
        5,
        5,
        2,
        5,
        2,
        5,
        2,
        2,
        5,
        2
      ]
    ],
    "return": true
  },
  {
    "args": [
      [
        1,
        2,
        2,
        1,
        2,
        2
      ]
    ],
    "return": true
  },
  {
    "args": [
      [
        1,
        2,
        2,
        2,
        1,
        2,
        2,
        2,
        1,
        2,
        2,
        2
      ]
    ],
    "return": true
  },
  {
    "args": [
      [
        1,
        2,
        1,
        2,
        1,
        2
      ]
    ],
    "return": true
  }
]
```

## Credits

Found on Edabit: [The Complete Bracelet](https://edabit.com/challenge/aMTXfakahQ45oZbJP)
