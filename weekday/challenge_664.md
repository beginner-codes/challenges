# Challenge 664 - Domino Chain

You were playing with dominos and concluded that:

- If the first domino is pushed over, it will tip the next domino to its right.
- The reaction will stop if a domino is already tipped over or if there is an empty space.

Create a function which takes a string which represents a line of dominos and returns the string after the domino chain reaction.

- `"|"` represents a standing domino.
- `"/"` represents a tripped domino.
- `" "` represents an empty space.

## Examples
```javascript
domino_chain("||| ||||//| |/") ➞ "/// ||||//| |/"
// A space will stop the reaction.

domino_chain("||//||") ➞ "////||"
// An already tripped domino will stop the reaction.

domino_chain("||||") ➞ "////"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def domino_chain(dominos: str) -> str:
    return ""  # Put your code here!!!


test(664, domino_chain)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            " |"
        ],
        "return": " |"
    },
    {
        "args": [
            " "
        ],
        "return": " "
    },
    {
        "args": [
            "||||| |||"
        ],
        "return": "///// |||"
    },
    {
        "args": [
            "|||||/|||"
        ],
        "return": "//////|||"
    },
    {
        "args": [
            ""
        ],
        "return": ""
    }
]
```
## Credits

Found on Edabit: [Domino Chain](https://edabit.com/challenge/SaZodzHyFoSv9XKPX)
