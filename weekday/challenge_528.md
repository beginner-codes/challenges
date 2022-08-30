# Challenge 528 - Sort Words by Their Last Character 

Create a function that takes a string of words and return a string with the words sorted alphabetically by the their last characters.

## Examples
```python
sort_by_last("herb camera dynamic") ➞ "camera herb dynamic"

sort_by_last("stab traction artist approach") ➞ "stab approach traction artist"

sort_by_last("sample partner autonomy swallow trend") ➞ "trend sample partner swallow autonomy"
```
## Notes

- Tests consist of lowercase alphabetic characters (a-z) and spaces.
- If two words have the same last character, sort by the order they originally appeared.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def sort_by_last(words: str) -> str:
    return "" # Put your code here!!!


test(528, sort_by_last)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "dividend platform pupil conclusion silence breakfast"
        ],
        "return": "dividend silence pupil platform conclusion breakfast"
    },
    {
        "args": [
            "sample partner autonomy swallow trend"
        ],
        "return": "trend sample partner swallow autonomy"
    },
    {
        "args": [
            "card warrant opinion medium illustrate"
        ],
        "return": "card illustrate medium opinion warrant"
    },
    {
        "args": [
            "stab traction artist approach"
        ],
        "return": "stab approach traction artist"
    },
    {
        "args": [
            "introduce fashionable cause sacrifice reality"
        ],
        "return": "introduce fashionable cause sacrifice reality"
    }
]
```
## Credits

Found on Edabit: [Sort a String by Its Last Character](https://edabit.com/challenge/ic9aKYukaRH2MjDyk)
