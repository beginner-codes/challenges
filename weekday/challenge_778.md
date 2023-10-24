# Challenge 778 - Let's Meet!

From point A an object is moving towards point B at a constant velocity (km/hr). From point B another object is moving towards point A at constant velocity (km/hr). Knowing this and the distance between point A and B (in km), write a function that returns how much time passes until both objects meet.

Format the output like this:
```python
"2h 23min 34s"
```
## Examples
```python
lets_meet(100, 10, 30) ➞ "2h 30min 0s"

lets_meet(280, 70, 80) ➞ "1h 52min 0s"

lets_meet(90, 75, 65) ➞ "0h 38min 34s"
```
## Notes

- Seconds should be rounded down to the nearest whole number.

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


def lets_meet(distance: int, velocity_a: int, velocity_b: int) -> str:
    return ""  # Put your code here!!!


test(778, lets_meet)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            33,
            15,
            20
        ],
        "return": "0h 56min 34s"
    },
    {
        "args": [
            100,
            10,
            30
        ],
        "return": "2h 30min 0s"
    },
    {
        "args": [
            250,
            60,
            80
        ],
        "return": "1h 47min 8s"
    },
    {
        "args": [
            360,
            80,
            64
        ],
        "return": "2h 30min 0s"
    },
    {
        "args": [
            33,
            15,
            20
        ],
        "return": "0h 56min 34s"
    }
]
```

## Credits

Found on Edabit: [Let's Meet!](https://edabit.com/challenge/9SLvXXz8ED7B6joJg)
