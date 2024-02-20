# Challenge 826 - Musical Cadences

In music, cadences act as punctuation in musical phrases, and help to mark the end of phrases. Cadences are the two chords at the end of a phrase. The different cadences are as follows:

- `V` followed by `I` is a Perfect Cadence
- `IV` followed by `I` is a Plagal Cadence
- `V` followed by Any chord other than `I` is an Interrupted Cadence
- Any chord followed by `V` is an Imperfect Cadence

Create a function where given a chord progression as a list, return the type of cadence the phrase ends on.

## Examples
```python
find_cadence(["I", "IV", "V"]) ➞ "imperfect"

find_cadence(["ii", "V", "I"]) ➞ "perfect"

find_cadence(["I", "IV", "I", "V", "vi"]) ➞ "interrupted"
```
## Notes

- Return strings all in lowercase.
- Only focus on the last two chords of a progression.
- Return `"no cadence"` if none of the criteria match up.

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


def find_cadence(chords: list[str]) -> str:
    return ""  # Put your code here!!!


test(826, find_cadence)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                "I",
                "IV",
                "V"
            ]
        ],
        "return": "imperfect"
    },
    {
        "args": [
            [
                "V",
                "IV",
                "V",
                "I",
                "vi"
            ]
        ],
        "return": "no cadence"
    },
    {
        "args": [
            [
                "I",
                "IV",
                "I",
                "V",
                "IV"
            ]
        ],
        "return": "interrupted"
    },
    {
        "args": [
            [
                "V",
                "IV",
                "I"
            ]
        ],
        "return": "plagal"
    },
    {
        "args": [
            [
                "V",
                "IV",
                "V",
                "III",
                "vi"
            ]
        ],
        "return": "no cadence"
    }
]
```

## Credits

Found on Edabit: [Musical Cadences](https://edabit.com/challenge/eoSXSf4C3gTbNJJEr)
