# Challenge 501 - Basic E-Mail Validation

Create a function that accepts a string, checks if it's a valid email address and returns either `True` or `False`, depending on the evaluation.

- The string must contain an `@` character.
- The string must contain a `.` character.
- The `@` must have at least one character in front of it. (e.g. "b@beginner.codes" is valid while "@beginner.codes" is invalid.)
- The `.` and the `@` must be in the appropriate places. (e.g. "hello.email@com" is invalid while "john.smith@email.com" is valid.)
- If the string passes these tests, it's considered a valid email address.

## Examples
```python
validate_email("@gmail.com") ➞ False

validate_email("hello.gmail@com") ➞ False

validate_email("gmail") ➞ False

validate_email("hello@gmail") ➞ False

validate_email("hello@beginner.codes") ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def validate_email(email: str) -> bool:
    return False  # Put your code here!!!


test(501, validate_email)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "@beginner.codes"
        ],
        "return": false
    },
    {
        "args": [
            "@beginner"
        ],
        "return": false
    },
    {
        "args": [
            "matt@beginner.codes"
        ],
        "return": true
    },
    {
        "args": [
            ""
        ],
        "return": false
    },
    {
        "args": [
            "hello.gmail@com"
        ],
        "return": false
    },
    {
        "args": [
            "bill.gates@microsoft.com"
        ],
        "return": true
    },
    {
        "args": [
            "hello@email"
        ],
        "return": false
    },
    {
        "args": [
            "%^%$#%^%"
        ],
        "return": false
    },
    {
        "args": [
            "www.email.com"
        ],
        "return": false
    },
    {
        "args": [
            "email"
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Basic E-Mail Validation](https://edabit.com/challenge/TBCujkw9D8hrEgFc4)
