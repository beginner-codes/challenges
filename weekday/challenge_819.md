# Challenge 819 - The Snake — Area Filling

This challenge is based on the classic videogame "Snake".

Assume the game screen is an `n * n` square, and the snake starts the game with length 1 (i.e. just the head) positioned on the top left corner.

In this version of the game, the length of the snake doubles each time it eats food (e.g. if the length is 4, after eating it becomes 8).

Create a function that takes the side length of the game screen and returns the number of times the snake can eat before it runs out of space on the game screen.

## Examples
```python
snake_fill(3) ➞ 3

snake_fill(6) ➞ 5

snake_fill(24) ➞ 9
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


def snake_fill(size: int) -> int:
    return 0  # Put your code here!!!


test(819, snake_fill)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            3
        ],
        "return": 3
    },
    {
        "args": [
            6
        ],
        "return": 5
    },
    {
        "args": [
            900
        ],
        "return": 19
    },
    {
        "args": [
            1
        ],
        "return": 0
    },
    {
        "args": [
            8
        ],
        "return": 6
    }
]
```

## Credits

Found on Edabit: [The Snake — Area Filling](https://edabit.com/challenge/Y5Ji2HDnQTX7MxeHt)
