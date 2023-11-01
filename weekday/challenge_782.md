# Challenge 782 - Words to Sentence

Create a function that turns a list of words into a comma separated list, where the last word is separated by the word `"and"`.

## Examples
```python
words_to_sentence(["coding"]) ➞ "coding"

words_to_sentence(["Hello", "", "Bye"]) ➞ "Hello and Bye"

words_to_sentence(["Hello", "Bye", "See you soon"]) ➞ "Hello, Bye and See you soon"
```
## Notes

- Null values, empty lists, or lists with only empty or Null values should return an empty string: `""`

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


def words_to_sentence(words: list[str]) -> str:
    return ""  # Put your code here!!!


test(782, words_to_sentence)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                "one",
                "",
                "three"
            ]
        ],
        "return": "one and three"
    },
    {
        "args": [
            [
                "one",
                "two",
                "three",
                "four"
            ]
        ],
        "return": "one, two, three and four"
    },
    {
        "args": [
            [
                ""
            ]
        ],
        "return": ""
    },
    {
        "args": [
            null
        ],
        "return": ""
    },
    {
        "args": [
            [
                "one",
                "two",
                "",
                "four"
            ]
        ],
        "return": "one, two and four"
    }
]
```

## Credits

Found on Edabit: [Words to Sentence](https://edabit.com/challenge/GP6CEr9a5CMqPHY7C)
