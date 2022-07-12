# Challenge 464 - Count the Smiley Faces :)

Create a function that takes a list of strings and return the number of smiley faces contained within it. These are the components that make up a valid smiley:

- A smiley has eyes. Eyes can be `:` or `;`.
- A smiley has a nose, but it doesn't have to. A nose can be `-` or `~`.
- A smiley has a mouth which can be `)` or `D`.
- No other characters are allowed except for those mentioned above.

## Examples
```python
count_smileys([":)", ";(", ";}", ":-D"]) ➞ 2

count_smileys([";D", ":-(", ":-)", ";~)"]) ➞ 3

count_smileys([";]", ":[", ";*", ":$", ";-D"]) ➞ 1
```
## Notes

- An empty list should return `0`.
- Noses are optional (e.g. `:)` and `:-)` are both valid).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def count_smileys(faces: list[str]) -> int:
    return 0  # Put your code here!!!


test(464, count_smileys)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                ":)",
                ";(",
                ";}",
                ":-D"
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                ";D",
                ":-(",
                ":-)",
                ";~)"
            ]
        ],
        "return": 3
    },
    {
        "args": [
            [
                ";]",
                ":[",
                ";*",
                ":$",
                ";-D"
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                ";(",
                ":>",
                ":}",
                ":]"
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                ":)",
                ":)",
                ":)",
                ":)",
                ":)",
                ":)",
                ":)",
                ":)",
                ":)",
                ":)",
                ":)",
                ":)",
                ":)"
            ]
        ],
        "return": 13
    },
    {
        "args": [
            [
                ":)",
                ":(",
                ":D",
                ":O",
                ":;"
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                ":-)",
                ";~D",
                ":-D",
                ":_D"
            ]
        ],
        "return": 3
    },
    {
        "args": [
            [
                ":---)",
                "))",
                ";~~D",
                ";D"
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                ";~)",
                ":)",
                ":-)",
                ":--)"
            ]
        ],
        "return": 3
    },
    {
        "args": [
            [
                ":o)",
                ":--D",
                ";-~)"
            ]
        ],
        "return": 0
    },
    {
        "args": [
            []
        ],
        "return": 0
    }
]
```
## Credits

Found on Edabit: [Count the Smiley Faces :)](https://edabit.com/challenge/gfo2RDnW7atsvQqnY)
