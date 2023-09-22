# Challenge 756 - The Empty Square Sequence

In the diagrams below there are squares of X's and empty spaces.
```
XX    X..X    X....X
XX    .XX.    .X..X.
      .XX.    ..XX..
      X..X    ..XX..
              .X..X.
              X....X
```
Create a function that takes a step (which is half the width of the square) and returns the amount of empty spaces. The diagram shows the squares with step 1, 2 and 3. The return value is the number of spaces not on a diagonal, which is 0 for the first square, 8 for the second, and 24 for the third.

## Examples
```python
empty_spaces(1) ➞ 0

empty_spaces(3) ➞ 24

empty_spaces(10) ➞ 360
```
## Notes

- Test input will always be a positive integer.
- The width of the square will always be even.

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


def empty_spaces(step: int) -> int:
    return 0  # Put your code here!!!


test(756, empty_spaces)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            10
        ],
        "return": 360
    },
    {
        "args": [
            1
        ],
        "return": 0
    },
    {
        "args": [
            3
        ],
        "return": 24
    },
    {
        "args": [
            19
        ],
        "return": 1368
    },
    {
        "args": [
            60
        ],
        "return": 14160
    }
]
```

## Credits

Found on Edabit: [The Empty Square Sequence](https://edabit.com/challenge/MeScMZ7GqAgyfvNKp)
