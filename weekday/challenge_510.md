# Challenge 510 - Chat Room Status

Write a function that returns the number of users in a chatroom based on the following rules:

- If there is no one, return `"no one online"`.
- If there is `1` person, return `"user1 online"`.
- If there are `2` people, return `"user1 and user2 online"`.
- If there are `>2` people, return the first two names and add `"and n-2 more online"`.

For example, if there are `5` users, return:

> `"user1, user2 and 3 more online"`

## Examples
```python
chatroom_status([]) ➞ "no one online"

chatroom_status(["paRIE_to"]) ➞ "paRIE_to online"

chatroom_status(["s234f", "mailbox2"]) ➞ "s234f and mailbox2 online"

chatroom_status(["pap_ier44", "townieBOY", "panda321", "motor_bike5", "sandwichmaker833", "violinist91"])
➞ "pap_ier44, townieBOY and 4 more online"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def chatroom_status(users: list[str]) -> str:
    return ""  # Put your code here!!!


test(510, chatroom_status)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            []
        ],
        "return": "no one online"
    },
    {
        "args": [
            [
                "becky325"
            ]
        ],
        "return": "becky325 online"
    },
    {
        "args": [
            [
                "becky325",
                "malcolm888"
            ]
        ],
        "return": "becky325 and malcolm888 online"
    },
    {
        "args": [
            [
                "becky325",
                "malcolm888",
                "fah32fa"
            ]
        ],
        "return": "becky325, malcolm888 and 1 more online"
    },
    {
        "args": [
            [
                "paRIE_to"
            ]
        ],
        "return": "paRIE_to online"
    }
]
```
## Credits

Found on Edabit: [Chat Room Status](https://edabit.com/challenge/PwGFjiSG3kXzp8rjw)
