# Challenge 824 - C\*ns\*r\*d Str\*ngs

Someone has attempted to censor my strings by replacing every vowel with a `*`, `l*k* th*s`. Luckily, I've been able to find the vowels that were removed.

Given a censored string and a string of the censored vowels, return the original uncensored string.

## Example
```python
uncensor("Wh*r* d*d my v*w*ls g*?", "eeioeo") ➞ "Where did my vowels go?"

uncensor("abcd", "") ➞ "abcd"

uncensor("*PP*RC*S*", "UEAE") ➞ "UPPERCASE"
```
## Notes

- The vowels are given in the correct order.
- The number of vowels will match the number of * characters in the censored string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def uncensor(message: str, vowels: str) -> str:
    return ""  # Put your code here!!!


test(824, uncensor)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "*l*ph*nt",
            "Eea"
        ],
        "return": "Elephant"
    },
    {
        "args": [
            "abcd",
            ""
        ],
        "return": "abcd"
    },
    {
        "args": [
            "Ch**s*, Gr*mm*t -- ch**s*",
            "eeeoieee"
        ],
        "return": "Cheese, Grommit -- cheese"
    },
    {
        "args": [
            "*PP*RC*S*",
            "UEAE"
        ],
        "return": "UPPERCASE"
    },
    {
        "args": [
            "Wh*r* d*d my v*w*ls g*?",
            "eeioeo"
        ],
        "return": "Where did my vowels go?"
    }
]
```

## Credits

Found on Edabit: [C\*ns\*r\*d Str\*ngs](https://edabit.com/challenge/ehyZvt6AJF4rKFfXT)
