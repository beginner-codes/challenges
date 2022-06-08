# Challenge 472 - Missing Letters

Given a string containing unique letters, return a sorted string with the letters that don't appear in the string.

## Examples

get_missing_letters("abcdefgpqrstuvwxyz") ➞ "hijklmno"

get_missing_letters("zyxwvutsrq") ➞ "abcdefghijklmnop"

get_missing_letters("abc") ➞ "defghijklmnopqrstuvwxyz"

get_missing_letters("abcdefghijklmnopqrstuvwxyz") ➞ ""

## Notes

- The combination of both strings should be `26` elements long, including all the letters in the alphabet.
- Letters will all be in lowercase.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def get_missing_letters(letters: str) -> str:
    return ""  # Put your code here!!!


test(472, get_missing_letters)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "abcdefgpqrstuvwxyz"
        ],
        "return": "hijklmno"
    },
    {
        "args": [
            "zyxwvutsrq"
        ],
        "return": "abcdefghijklmnop"
    },
    {
        "args": [
            ""
        ],
        "return": "abcdefghijklmnopqrstuvwxyz"
    },
    {
        "args": [
            "abcdefghijklmnopqrstuvwxyz"
        ],
        "return": ""
    },
    {
        "args": [
            "qinjwm"
        ],
        "return": "abcdefghkloprstuvxyz"
    },
    {
        "args": [
            "luiqtkgwzheapr"
        ],
        "return": "bcdfjmnosvxy"
    },
    {
        "args": [
            "qankj"
        ],
        "return": "bcdefghilmoprstuvwxyz"
    },
    {
        "args": [
            "bawgeuskmfcrpodnxztviy"
        ],
        "return": "hjlq"
    },
    {
        "args": [
            "gdpna"
        ],
        "return": "bcefhijklmoqrstuvwxyz"
    },
    {
        "args": [
            "hbi"
        ],
        "return": "acdefgjklmnopqrstuvwxyz"
    }
]
```
## Credits

Found on Edabit: [Missing Letters](https://edabit.com/challenge/bGRYmEZvzWFK2sbek)
