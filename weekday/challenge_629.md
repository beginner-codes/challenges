# Challenge 629 - Likes vs. Dislikes

YouTube currently displays a like and a dislike button, allowing you to express your opinions about particular content. It's set up in such a way that you cannot like and dislike a video at the same time.

There are two other interesting rules to be noted about the interface:

- Pressing a button, which is already active, will undo your press.
- If you press the like button after pressing the dislike button, the like button overwrites the previous "dislike" state. The same is true for the other way round.

Create a function that takes in a list of button inputs and returns the final state.

## Examples
```python
like_or_dislike(["Dislike"]) ➞ "Dislike"

like_or_dislike(["Like", "Like"]) ➞ "Nothing"

like_or_dislike(["Dislike", "Like"]) ➞ "Like"

like_or_dislike(["Like", "Dislike", "Dislike"]) ➞ "Nothing"
```
## Notes

- If no button is currently active, return `"Nothing"`.
- If the list is empty, return `"Nothing"`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def like_or_dislike(buttons: list[str]) -> str:
    return ""  # Put your code here!!!


test(629, like_or_dislike)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            []
        ],
        "return": "Nothing"
    },
    {
        "args": [
            [
                "Dislike",
                "Like",
                "Dislike"
            ]
        ],
        "return": "Dislike"
    },
    {
        "args": [
            [
                "Dislike",
                "Dislike"
            ]
        ],
        "return": "Nothing"
    },
    {
        "args": [
            [
                "Like",
                "Like",
                "Dislike",
                "Like",
                "Dislike",
                "Like",
                "Like",
                "Like"
            ]
        ],
        "return": "Like"
    },
    {
        "args": [
            [
                "Dislike"
            ]
        ],
        "return": "Dislike"
    }
]
```
## Credits

Found on Edabit: [Likes vs. Dislikes](https://edabit.com/challenge/egMp3GWyN8TPptbZA)
