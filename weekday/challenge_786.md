# Challenge 786 - Mexican Wave Simulator

The wave (known as a Mexican wave in the English-speaking world outside of North America) is an example of metachronal rhythm achieved in a packed stadium when successive groups of spectators briefly stand, yell, and raise their arms.

Create a function that takes a string and turns it into a Mexican Wave.

## Examples
```python
wave("just do it") ➞ ["Just do it", "jUst do it", "juSt do it", "jusT do it", "just Do it", "just dO it", "just do It", "just do iT"]

wave(" ") ➞ []
```
## Notes

- Ignore spaces (they are considered empty seats)
- An empty string should return an empty list

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


def wave(string: str) -> list[str]:
    return []  # Put your code here!!!


test(786, wave)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            " blue"
        ],
        "return": [
            " Blue",
            " bLue",
            " blUe",
            " bluE"
        ]
    },
    {
        "args": [
            "dogs cats pigs"
        ],
        "return": [
            "Dogs cats pigs",
            "dOgs cats pigs",
            "doGs cats pigs",
            "dogS cats pigs",
            "dogs Cats pigs",
            "dogs cAts pigs",
            "dogs caTs pigs",
            "dogs catS pigs",
            "dogs cats Pigs",
            "dogs cats pIgs",
            "dogs cats piGs",
            "dogs cats pigS"
        ]
    },
    {
        "args": [
            ""
        ],
        "return": []
    },
    {
        "args": [
            "g"
        ],
        "return": [
            "G"
        ]
    }
]
```

## Credits

Found on Edabit: [Mexican Wave Simulator](https://edabit.com/challenge/Cm9fAzNkWWdzit23N)
