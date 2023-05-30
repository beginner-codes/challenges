# Challenge 673 - Choosing a Fuse

A fuse melts when a current in an electrical device exceeds the fuse's rating, breaking the circuit and preventing the heat from building up too much (which can cause a fire). The ideal fuse to choose is higher than the device's current output, yet as close as possible to it as well.

Given a list of fuse ratings, and the device's current output, return which of the fuses is the best for the device.

## Examples
```python
choose_fuse(["3V", "5V", "12V"], "4.5V") ➞ "5V"

choose_fuse(["5V", "14V", "2V"], "5.5V") ➞ "14V"

choose_fuse(["17V", "15V", "12V"], "9V") ➞ "12V"
```
## Notes

- You will be given three possible ratings in voltage.
- Fuses may not be in a sorted order.
- Assume that there is a valid fuse in every test case

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def choose_fuse(fuses: list[str], voltage: str) -> str:
    return ""  # Put your code here!!!


test(673, choose_fuse)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "1V",
                "2V",
                "3V"
            ],
            "2.5V"
        ],
        "return": "3V"
    },
    {
        "args": [
            [
                "17V",
                "15V",
                "12V"
            ],
            "9V"
        ],
        "return": "12V"
    },
    {
        "args": [
            [
                "5V",
                "14V",
                "2V"
            ],
            "5.5V"
        ],
        "return": "14V"
    },
    {
        "args": [
            [
                "3V",
                "5V",
                "12V"
            ],
            "4.5V"
        ],
        "return": "5V"
    },
    {
        "args": [
            [
                "7V",
                "135V",
                "12V"
            ],
            "9.5V"
        ],
        "return": "12V"
    }
]
```
## Credits

Found on Edabit: [Choosing a Fuse](https://edabit.com/challenge/HDGiiCmSgJeeu3388)
