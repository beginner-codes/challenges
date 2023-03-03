# Challenge 617 - Sort Words by a String

Create a function that sorts words by a given string.

## Examples
```python
sort_by_string(["poof", "floof", "loop"], "flatp")
➞ ["floof", "loop", "poof"]

sort_by_string(["small", "big", "medium"], "sazymtb")
➞ ["small", "medium", "big"]

sort_by_string(["apple", "banana", "cherry", "date"], "dbca")
➞ ["date", "banana", "cherry", "apple"]
```
## Notes

- The string may have excess letters.
- There will be unique starting letters in each list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sort_by_string(words: list[str], sort_by: str) -> list[str]:
    return []  # Put your code here!!!


test(617, sort_by_string)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "small",
                "big",
                "medium"
            ],
            "sazymtb"
        ],
        "return": [
            "small",
            "medium",
            "big"
        ]
    },
    {
        "args": [
            [
                "poof",
                "floof",
                "loop"
            ],
            "flatp"
        ],
        "return": [
            "floof",
            "loop",
            "poof"
        ]
    },
    {
        "args": [
            [
                "apple",
                "banana",
                "cherry",
                "date"
            ],
            "dbca"
        ],
        "return": [
            "date",
            "banana",
            "cherry",
            "apple"
        ]
    },
    {
        "args": [
            [
                "yellow",
                "phone",
                "book"
            ],
            "abcdpy"
        ],
        "return": [
            "book",
            "phone",
            "yellow"
        ]
    }
]
```
## Credits

Found on Edabit: [Sort Words by a String](https://edabit.com/challenge/hjZTbJNzKiSxTtbik)
