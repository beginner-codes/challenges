# Challenge 500 - Maskify the String

Usually when you sign up for an account to buy something, your credit card number, phone number or answer to a secret question is partially obscured in some way. Since someone could look over your shoulder, you don't want that shown on your screen. Hence, the website masks these strings.

Your task is to create a function that takes a string, transforms all but the last four characters into `"#"` and returns the new masked string.

## Examples
```python
maskify("4556364607935616") ➞ "############5616"

maskify("64607935616") ➞ "#######5616"

maskify("1") ➞ "1"

maskify("") ➞ ""
```
## Notes

- The `maskify` function must accept a string of any length.
- An empty string should return an empty string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def maskify(cc_number: str) -> str:
    return ""  # Put your code here!!!


test(500, maskify)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "4556364607935616"
        ],
        "return": "############5616"
    },
    {
        "args": [
            "64607935616"
        ],
        "return": "#######5616"
    },
    {
        "args": [
            "1"
        ],
        "return": "1"
    },
    {
        "args": [
            ""
        ],
        "return": ""
    },
    {
        "args": [
            "tBy>L/cMe+?<j:6n;C~H"
        ],
        "return": "################;C~H"
    },
    {
        "args": [
            "12"
        ],
        "return": "12"
    },
    {
        "args": [
            "8Ikhlf6yoxPOwi5cB014eWbRumj7vJ"
        ],
        "return": "##########################j7vJ"
    },
    {
        "args": [
            "123"
        ],
        "return": "123"
    },
    {
        "args": [
            "2673951408"
        ],
        "return": "######1408"
    },
    {
        "args": [
            "1234"
        ],
        "return": "1234"
    }
]
```
## Credits

Found on Edabit: [Maskify the String](https://edabit.com/challenge/xRzyWsdzMEeGqsJMK)
