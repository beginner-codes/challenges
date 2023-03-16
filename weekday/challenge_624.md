# Challenge 624 - Author Sorting

Create a function which sorts a list of authors by their last name. The list may include initials and full names, but note that there will be a mix of upper and lowercase.

## Examples
```python
sort_authors(["J. K. Rowling", "w. s.", "lewis carroll", "M. M."]) ➞ ["lewis carroll", "M. M.", "J. K. Rowling", "w. s."]

sort_authors(["J. L.", "J. B. priestley", "L. C.", "Suzanne Collins"]) ➞ ["L. C.", "Suzanne Collins", "J. L.", "J. B. priestley"]
```
## Notes

- If two surnames begin with the same letter, return them in the order they appeared.
- Note how there are spaces between each of the initials.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sort_authors(authors: list[str]) -> list[str]:
    return []  # Put your code here!!!


test(624, sort_authors)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "J. L.",
                "J. B. Priestley",
                "L. C.",
                "Suzanne Collins"
            ]
        ],
        "return": [
            "L. C.",
            "Suzanne Collins",
            "J. L.",
            "J. B. Priestley"
        ]
    },
    {
        "args": [
            [
                "J. K. Rowling",
                "w. s.",
                "lewis carroll",
                "M. M."
            ]
        ],
        "return": [
            "lewis carroll",
            "M. M.",
            "J. K. Rowling",
            "w. s."
        ]
    },
    {
        "args": [
            [
                "J. L.",
                "J. B. Priestley",
                "L. C.",
                "suzanne collins",
                "W. S."
            ]
        ],
        "return": [
            "L. C.",
            "suzanne collins",
            "J. L.",
            "J. B. Priestley",
            "W. S."
        ]
    },
    {
        "args": [
            [
                "J. L.",
                "J. B. priestley",
                "L. C.",
                "Suzanne Collins"
            ]
        ],
        "return": [
            "L. C.",
            "Suzanne Collins",
            "J. L.",
            "J. B. priestley"
        ]
    },
    {
        "args": [
            [
                "J. K. Rowling",
                "W. S.",
                "Lewis Carroll",
                "M. M."
            ]
        ],
        "return": [
            "Lewis Carroll",
            "M. M.",
            "J. K. Rowling",
            "W. S."
        ]
    }
]
```
## Credits

Found on Edabit: [Author Sorting](https://edabit.com/challenge/TjozEDjS7u5udR942)
