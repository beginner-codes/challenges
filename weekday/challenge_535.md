# Challenge 535 - Parity Bit Validation

Parity bits are used as very simple checksum to ensure that binary data isn't corrupted during transit. Here's how they work:

- If a binary string has an odd number of `1`s, the parity bit is a `1`.
- If a binary string has an even number of `1`s, the parity bit is a `0`.
- The parity bit is appended to the end of the binary string.

Create a function that validates whether a binary string is valid, using parity bits.

## Worked Example
```python
validate_binary("10110010") ➞ True

# The last digit is the parity bit.
# 0 is the last digit.
# 0 means that there should be an even number of 1s.
# There are four 1s.
# Return True.
```
## Examples
```python
validate_binary("00101101") ➞ True

validate_binary("11000000") ➞ True

validate_binary("11000001") ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def validate_binary(byte: str) -> bool:
    return False # Put your code here!!!


test(535, validate_binary)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "00101101"
        ],
        "return": true
    },
    {
        "args": [
            "10010010"
        ],
        "return": false
    },
    {
        "args": [
            "11000001"
        ],
        "return": false
    },
    {
        "args": [
            "11000000"
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Parity Bit Validation](https://edabit.com/challenge/DcXTvFs7Zvc3PDTzX)
