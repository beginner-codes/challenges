# Challenge 638 - String to Dictionary

Create a function that takes a list of strings and returns a dictionary.

## Examples
```python
str_to_dict(["1=one", "2=two", "3=three", "4=four"]) ➞ {"1": "one", "2": "two", "3": "three", "4": "four"}

str_to_dict(["dog=bark", "cat=meow", "cow=moo"]) ➞ {"dog": "bark", "cat": "meow", "cow": "moo"}

str_to_dict(["bob=human", "lola=dog", "mittens=cat", "todd=frog"]) ➞ {"bob": "human", "lola": "dog", "mittens": "cat", "todd": "frog"}
```
## Notes

- Key and value with be separated with `=`.
- Input list will be of various lengths.
- The key will be the first element in the string and the value with be the second.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def str_to_dict(items: str) -> dict[str, str]:
    return {}  # Put your code here!!!


test(638, str_to_dict)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "greeting=Hello There!",
                "dismissal=Goodbye!",
                "thanks=Thank you!"
            ]
        ],
        "return": {
            "greeting": "Hello There!",
            "dismissal": "Goodbye!",
            "thanks": "Thank you!"
        }
    },
    {
        "args": [
            [
                "name=bob",
                "balance=500",
                "salary=10000",
                "friends=0"
            ]
        ],
        "return": {
            "name": "bob",
            "balance": "500",
            "salary": "10000",
            "friends": "0"
        }
    },
    {
        "args": [
            [
                "1=one",
                "2=two",
                "3=three",
                "4=four"
            ]
        ],
        "return": {
            "1": "one",
            "2": "two",
            "3": "three",
            "4": "four"
        }
    },
    {
        "args": [
            [
                "bob=human",
                "lola=dog",
                "mittens=cat",
                "todd=frog"
            ]
        ],
        "return": {
            "bob": "human",
            "lola": "dog",
            "mittens": "cat",
            "todd": "frog"
        }
    },
    {
        "args": [
            [
                "dog=bark",
                "cat=meow",
                "cow=moo"
            ]
        ],
        "return": {
            "dog": "bark",
            "cat": "meow",
            "cow": "moo"
        }
    }
]
```
## Credits

Found on Edabit: [String to Dictionary](https://edabit.com/challenge/iG5vcwd282T4t7h6r)
