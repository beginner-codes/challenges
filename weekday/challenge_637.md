# Challenge 637 - Robot Path 🤖

There is a simple robot that is navigated using a series of North, East, South, and West commands. Each command moves the robot one step in the given direction. The robot can only end at one of two destinations:

- Destination No. 1: `e, n, e, e, n`
- Destination No. 2: `w, n, w, n, w, w, n`

Create a function that takes a list of commands and returns True if the robot reaches any of the destinations, False otherwise.

## Examples
```python
robot_path(["s", "e", "e", "n", "n", "e", "n"]) ➞ True
# Robot will end up at destination no. 1

robot_path(["n", "e", "s", "w", "n", "e", "s", "w", "w", "s", "n", "e"]) ➞ False
# Robot will be lost somewhere

robot_path(["n", "s", "n", "n", "e", "n", "w", "w", "s", "w", "w", "w", "n"]) ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def robot_path(commmands: list[str]) -> bool:
    return False  # Put your code here!!!


test(637, robot_path)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "n",
                "s",
                "n",
                "n",
                "n",
                "e",
                "n",
                "w",
                "n",
                "w",
                "s",
                "w",
                "w",
                "w",
                "n"
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                "n",
                "s",
                "n",
                "s",
                "n",
                "s",
                "n",
                "s",
                "n",
                "s",
                "n",
                "s",
                "n",
                "s",
                "e",
                "w",
                "w"
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                "s",
                "e",
                "e",
                "n",
                "n",
                "e",
                "n"
            ]
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Robot Path 🤖](https://edabit.com/challenge/towwrEJ7zr8xKGSr5)
