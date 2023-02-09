# Challenge 602 - An Absolute

Given a sentence, create a function that replaces every "a"/"an" that's used as an article with "an absolute". It should return the same string without any change if it doesn't have any "a".

## Examples
```python
absolute("I am a champion!!!") ➞ "I am an absolute champion!!!"

absolute("Such an amazing bowler.") ➞ "Such an amazing bowler."

absolute("A man with no haters.") ➞ "An absolute man with no haters."
```
## Notes

- Watch for uppercase letters.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def absolute(sentence: str) -> str:
    return ""  # Put your code here!!!


test(602, absolute)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "Such an amazing bowler."
        ],
        "return": "Such an amazing bowler."
    },
    {
        "args": [
            "A man with no haters."
        ],
        "return": "An absolute man with no haters."
    },
    {
        "args": [
            "A hero of the leaf"
        ],
        "return": "An absolute hero of the leaf"
    },
    {
        "args": [
            "I am a champion!!!"
        ],
        "return": "I am an absolute champion!!!"
    },
    {
        "args": [
            "That place is such a beauty"
        ],
        "return": "That place is such an absolute beauty"
    }
]
```
## Credits

Found on Edabit: [An Absolute](https://edabit.com/challenge/MYZu2j5zKndMB2zdg)
