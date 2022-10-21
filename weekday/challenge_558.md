# Challenge 558 - Word Nests

A word nest is created by taking a starting word, and generating a new string by placing the word inside itself. This process is then repeated.

Nesting 3 times with the word `"incredible"`:
```
start  = incredible
first  = incre|incredible|dible
second = increin|incredible|credibledible
third  = increinincr|incredible|ediblecredibledible
The final nest is "increinincrincredibleediblecredibledible" (depth = 3).
```
Given a starting word and the final word nest, return the depth of the word nest.

## Examples
```python
word_nest("floor", "floor") ➞ 0

word_nest("code", "cocodccococodededeodeede") ➞ 5

word_nest("incredible", "increinincrincredibleediblecredibledible") ➞ 3
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def word_nest(word: str, nest: str) -> int:
    return 0 # Put your code here!!!


test(558, word_nest)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "profession",
            "profesprofessionsion"
        ],
        "return": 1
    },
    {
        "args": [
            "continuous",
            "contcontcontinuoconcocontinuousntinuoustinuoususinuousinuous"
        ],
        "return": 5
    },
    {
        "args": [
            "home",
            "hohohohhohohhhohhomeomemeomeomememeomemememe"
        ],
        "return": 10
    },
    {
        "args": [
            "sweater",
            "sweatsweswsweatereateraterer"
        ],
        "return": 3
    },
    {
        "args": [
            "relieve",
            "relierelierelrelierrelieveelieveveieveveve"
        ],
        "return": 5
    },
    {
        "args": [
            "caller",
            "callcacacalccallcacaccallerallerllerllererallerlerllerllerer"
        ],
        "return": 9
    },
    {
        "args": [
            "measure",
            "measumememeasumemmeasmmeasureeasureureeasureasurereasureasurere"
        ],
        "return": 8
    },
    {
        "args": [
            "ruin",
            "rurrurrrrrrururuinininuinuinuinuinuininuinin"
        ],
        "return": 10
    }
]
```
## Credits

Found on Edabit: [Word Nests](https://edabit.com/challenge/EjjBGn7hkmhgxqJej)
