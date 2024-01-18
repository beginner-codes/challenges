# Challenge 806 - Enter the Matrix

In this challenge, you have to obtain a sentence from the elements of a given matrix. In the matrix, each word of the sentence follows a columnar order from the top to the bottom, instead of the usual left-to-right order: it's time for transposition!

Given a matrix, implement a function that returns the complete sentence as a string, with the words separated by a space between them.

## Examples
```python
transpose_matrix([
  ["Enter"],
  ["the"],
  ["Matrix!"]
]) ➞ "Enter the Matrix!"

transpose_matrix([
  ["The", "are"],
  ["columns", "rows."]
]) ➞ "The columns are rows."

transpose_matrix([
  ["You", "the"],
  ["must", "table"],
  ["transpose", "order."]
]) ➞ "You must transpose the table order."
```
## Notes

- All given matrices are regular, as to say that each column has the same length.
- Punctuation is already given, you just have to add the spaces in the returned string.

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


def transpose_matrix(matrix: list[list[str]]) -> str:
    return ""  # Put your code here!!!


test(806, transpose_matrix)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                [
                    "Enter"
                ],
                [
                    "the"
                ],
                [
                    "Matrix."
                ]
            ]
        ],
        "return": "Enter the Matrix."
    },
    {
        "args": [
            [
                [
                    "As",
                    "human"
                ],
                [
                    "long",
                    "race"
                ],
                [
                    "as",
                    "will"
                ],
                [
                    "Matrix",
                    "never"
                ],
                [
                    "exists,",
                    "be"
                ],
                [
                    "the",
                    "free."
                ]
            ]
        ],
        "return": "As long as Matrix exists, the human race will never be free."
    },
    {
        "args": [
            [
                [
                    "If",
                    "killed",
                    "you"
                ],
                [
                    "you",
                    "in",
                    "die"
                ],
                [
                    "are",
                    "Matrix",
                    "here?"
                ]
            ]
        ],
        "return": "If you are killed in Matrix you die here?"
    }
]
```

## Credits

Found on Edabit: [Enter the Matrix](https://edabit.com/challenge/kdhgEC2ECXAfoXWQP)
