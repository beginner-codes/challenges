# Challenge 588 - No Yelling

Create a function that transforms sentences ending with multiple question marks `?` or exclamation marks `!` into a sentence only ending with one without changing punctuation in the middle of the sentences.

## Examples
```python
no_yelling("What went wrong?????????") ➞ "What went wrong?"

no_yelling("Oh my goodness!!!") ➞ "Oh my goodness!"

no_yelling("I just!!! can!!! not!!! believe!!! it!!!") ➞ "I just!!! can!!! not!!! believe!!! it!"
# Only change repeating punctuation at the end of the sentence.

no_yelling("Oh my goodness!") ➞ "Oh my goodness!"
# Do not change sentences where there exists only one or zero exclamation marks/question marks.

no_yelling("I just cannot believe it.") ➞ "I just cannot believe it."
```
## Notes

- Only change ending punctuation - keep the exclamation marks or question marks in the middle of the sentence the same.
- Don't worry about mixed punctuation (no cases that end in something like `?!??!`).
- Keep sentences that do not have question/exclamation marks the same.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def no_yelling(sentence: str) -> str:
    return ""  # Put your code here!!!


test(588, no_yelling)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "Oh my goodness!"
        ],
        "return": "Oh my goodness!"
    },
    {
        "args": [
            "I just!!! can!!! not!!! believe!!! it!!!"
        ],
        "return": "I just!!! can!!! not!!! believe!!! it!"
    },
    {
        "args": [
            "That's a ton!! of cheese!!!!"
        ],
        "return": "That's a ton!! of cheese!"
    },
    {
        "args": [
            "Oh my goodness!!!"
        ],
        "return": "Oh my goodness!"
    },
    {
        "args": [
            "WHAT?"
        ],
        "return": "WHAT?"
    }
]
```
## Credits

Found on Edabit: [No Yelling](https://edabit.com/challenge/hAsdEPWwufWoJos32)
