# Challenge 584 - How Many Unique Styles?

There are different styles of music and many albums exhibit multiple styles. Create a function that takes a list of musical styles from albums and returns how many styles are unique.

## Examples
```python
unique_styles([
  "Dub,Dancehall",
  "Industrial,Heavy Metal",
  "Techno,Dubstep",
  "Synth-pop,Euro-Disco",
  "Industrial,Techno,Minimal"
]) ➞ 9

unique_styles([
  "Soul",
  "House,Folk",
  "Trance,Downtempo,Big Beat,House",
  "Deep House",
  "Soul"
]) ➞ 7
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def unique_styles(albums: list[str]) -> int:
    return 0  # Put your code here!!!


test(584, unique_styles)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "Dub,Dancehall",
                "Industrial,Heavy Metal",
                "Techno,Dubstep",
                "Synth-pop,Euro-Disco",
                "Industrial,Techno,Minimal"
            ]
        ],
        "return": 9
    },
    {
        "args": [
            [
                "Soul",
                "House,Folk",
                "Trance,Downtempo,Big Beat,House",
                "Deep House",
                "Soul"
            ]
        ],
        "return": 7
    },
    {
        "args": [
            [
                "Black Metal,Avantgarde",
                "Funk",
                "Deep House,House",
                "Big Band",
                "Punk"
            ]
        ],
        "return": 7
    },
    {
        "args": [
            [
                "Funk",
                "Funk",
                "Funk",
                "Funk",
                "Funk"
            ]
        ],
        "return": 1
    }
]
```
## Credits

Found on Edabit: [How Many Unique Styles?](https://edabit.com/challenge/AvP94XqJvPjoMk5PT)
