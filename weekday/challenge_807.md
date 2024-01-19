# Challenge 807 - All About Strings

Create a function that, given a string with at least three characters, returns an array of its:

- Length
- First character
- Last character
- Middle character, if the string has an odd number of characters. Middle TWO characters, if the string has an even number of characters
- Index of the second occurrence of the second character in the format `"@ index #"` and `"not found"` if the second character doesn't occur again

## Examples
```python
all_about_strings("LASA") ➞ [4, "L", "A", "AS", "@ index 3"]

all_about_strings("Computer") ➞ [8, "C", "r", "pu", "not found"]

all_about_strings("Science") ➞ [7, "S", "e", "e", "@ index 5"]
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


def all_about_strings(string: str) -> list[int | str]:
    return []  # Put your code here!!!


test(807, all_about_strings)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "break"
        ],
        "return": [
            5,
            "b",
            "k",
            "e",
            "not found"
        ]
    },
    {
        "args": [
            "LASA"
        ],
        "return": [
            4,
            "L",
            "A",
            "AS",
            "@ index 3"
        ]
    },
    {
        "args": [
            "programming"
        ],
        "return": [
            11,
            "p",
            "g",
            "a",
            "@ index 4"
        ]
    },
    {
        "args": [
            "Science"
        ],
        "return": [
            7,
            "S",
            "e",
            "e",
            "@ index 5"
        ]
    },
    {
        "args": [
            "spring"
        ],
        "return": [
            6,
            "s",
            "g",
            "ri",
            "not found"
        ]
    }
]
```

## Credits

Found on Edabit: [All About Strings](https://edabit.com/challenge/pEozhEet5c8aFJdso)
