# Challenge 571 - Most Common Last Vowel

Create a function that takes in a sentence as input and returns the most common last vowel in the sentence as a single character string.

## Examples
```python
common_last_vowel("Hello World!") ➞ "o"

common_last_vowel("Watch the characters dance!") ➞ "e"

common_last_vowel("OOI UUI EEI AAI") ➞ "i"

```
## Notes

- `"y"` won't count as a vowel.
- Return outputs in lowercase.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def common_last_vowel(sentence: str) -> str:
    return ""  # Put your code here!!!


test(571, common_last_vowel)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "munch munch munch tasty tasty brunch"
        ],
        "return": "u"
    },
    {
        "args": [
            "Watch the characters dance!"
        ],
        "return": "e"
    },
    {
        "args": [
            "Hello World!"
        ],
        "return": "o"
    },
    {
        "args": [
            "OOI UUI EEI AAI"
        ],
        "return": "i"
    },
    {
        "args": [
            "amy and acts"
        ],
        "return": "a"
    }
]
```
## Credits

Found on Edabit: [Most Common Last Vowel](https://edabit.com/challenge/9Kuah39g997SvZmex)
