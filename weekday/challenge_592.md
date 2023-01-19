# Challenge 592 - Functioninator 8000

Create a function that takes a single word and does the following:

- Concatenates `"inator"` to the end if the word ends with a consonant, otherwise, concatenate `"-inator"` instead.
- Adds the word length of the original word to the end, followed by `"000"`.

## Examples
```python
inator_inator("Shrink") ➞ "Shrinkinator 6000"

inator_inator("Doom") ➞ "Doominator 4000"

inator_inator("EvilClone") ➞ "EvilClone-inator 9000"
```
## Notes

- For the purposes of this challenge, vowels will be `a`, `e`, `i`, `o` and `u` only.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def inator_inator(word: str) -> str:
    return ""  # Put your code here!!!


test(592, inator_inator)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "EvilClone"
        ],
        "return": "EvilClone-inator 9000"
    },
    {
        "args": [
            "a"
        ],
        "return": "a-inator 1000"
    },
    {
        "args": [
            "Doom"
        ],
        "return": "Doominator 4000"
    },
    {
        "args": [
            "Destroy"
        ],
        "return": "Destroyinator 7000"
    },
    {
        "args": [
            "foo"
        ],
        "return": "foo-inator 3000"
    }
]
```
## Credits

Found on Edabit: [Functioninator 8000](https://edabit.com/challenge/88RHBqSA84yT3fdLM)
