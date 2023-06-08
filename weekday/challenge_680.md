# Challenge 680 - Adding Up Letters

Create a function that takes a list of letters, and returns the "sum" of those letters.

To add two letters, take their number value, add them together, and convert it back together. For example, `a` would be 1, `b` would be 2, etc. So to add `b` and `c`, take `2 + 3 = 5`, and then get the fifth letter of the alphabet `e`.

So then `d + e + f` would be `4 + 5 + 6 = 15`, and the fifteenth letter is `o`, so that's what you return.

Letters can also wrap. Like with `y + c`, that's `25 + 3 = 28`, which doesn't exist. Consider that the 27th letter just wraps around and ends back up at `a`. With this logic, `y + c = b`. Don't just do `27 = 1` though, because you could end up with a much higher sum like 70.

## Examples
```py
add_letters(["a"]) ➞ "a"
add_letters(["a", "b"]) ➞ "c"
add_letters(["a", "b", "c"]) ➞ "f"
```
## Notes

- All letters given will be lowercase.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def add_letters(letters: list[str]) -> str:
    return ""  # Put your code here!!!


test(680, add_letters)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "a",
                "b",
                "c"
            ]
        ],
        "return": "f"
    },
    {
        "args": [
            [
                "a",
                "b"
            ]
        ],
        "return": "c"
    },
    {
        "args": [
            [
                "a",
                "b",
                "c",
                "d",
                "e",
                "f"
            ]
        ],
        "return": "u"
    },
    {
        "args": [
            [
                "z",
                "a"
            ]
        ],
        "return": "a"
    },
    {
        "args": [
            [
                "y",
                "c"
            ]
        ],
        "return": "b"
    }
]
```
## Credits

Found on Edabit: [Adding Up Letters](https://edabit.com/challenge/yKMxg88HGXmLhirht)
