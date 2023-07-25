# Challenge 712 - Numbers in Strings

Create a function that takes a list of strings and returns a list of the strings that contain numbers. If there are no strings containing numbers, return an empty list.

## Examples
```python
num_in_str(["1a", "a", "2b", "b"]) ➞ ["1a", "2b"]

num_in_str(["abc", "abc10"]) ➞ ["abc10"]

num_in_str(["abc", "ab10c", "a10bc", "bcd"]) ➞ ["ab10c", "a10bc"]

num_in_str(["this is a test", "test1"]) ➞ ["test1"]
```
## Notes

- The strings can contain any character, including white space. 

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def num_in_str(strings: list[str]) -> list[str]:
    return []  # Put your code here!!!


test(712, num_in_str)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "-/>",
                "10bc",
                "abc "
            ]
        ],
        "return": [
            "10bc"
        ]
    },
    {
        "args": [
            [
                "abc",
                "abc10"
            ]
        ],
        "return": [
            "abc10"
        ]
    },
    {
        "args": [
            [
                "this IS",
                "10xYZ",
                "xy2K77",
                "Z1K2W0",
                "xYz"
            ]
        ],
        "return": [
            "10xYZ",
            "xy2K77",
            "Z1K2W0"
        ]
    },
    {
        "args": [
            [
                "rct",
                "ABC",
                "Test",
                "xYz"
            ]
        ],
        "return": []
    },
    {
        "args": [
            [
                "abc",
                "ab10c",
                "a10bc",
                "bcd"
            ]
        ],
        "return": [
            "ab10c",
            "a10bc"
        ]
    },
    {
        "args": [
            [
                "1",
                "a",
                " ",
                "b"
            ]
        ],
        "return": [
            "1"
        ]
    }
]
```
## Credits

Found on Edabit: [Numbers in Strings](https://edabit.com/challenge/XYYdtkhGPXXJ3QQNB)
