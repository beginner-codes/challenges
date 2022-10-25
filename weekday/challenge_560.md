# Challenge 560 - Retrieve Name from Email Address

Create a function that takes an email address and returns the name in the address.

- The "name" is the letters/alphabetical characters before the `@` in the address.
- The "name" will not always be an actual name.
- Email addresses will end in something like `@domain.com`

## Examples
```python
get_name("yourname@example.com") ➞ "yourname"

get_name("john64@gmail.com") ➞ "john"

get_name("pamela78_Cole@hotmail.com") ➞ "pamelaCole"

get_name("Chickenlololol29@yahoo.com") ➞ "Chickenlololol"
```
## Notes

- Keep the original capitalization in the email address.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def get_name(email: str) -> str:
    return "" # Put your code here!!!


test(560, get_name)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "python$#$\"_guy@overtherainbow.net"
        ],
        "return": "pythonguy"
    },
    {
        "args": [
            "sars-CoV-2@pandemic.org"
        ],
        "return": "sarsCoV"
    },
    {
        "args": [
            "yourname@example.com"
        ],
        "return": "yourname"
    },
    {
        "args": [
            "john64@gmail.com"
        ],
        "return": "john"
    },
    {
        "args": [
            "e@ifdirmvsidso.jeksdjjcoa"
        ],
        "return": "e"
    },
    {
        "args": [
            "Mr.President2050@USofA.gov"
        ],
        "return": "MrPresident"
    },
    {
        "args": [
            "][:;><?/(*^%$E@br.uh"
        ],
        "return": "E"
    },
    {
        "args": [
            "a@b.c"
        ],
        "return": "a"
    }
]
```
## Credits

Found on Edabit: [Retrieve Name from Email Address](https://edabit.com/challenge/pDmDP9KhXmBTcScT6)
