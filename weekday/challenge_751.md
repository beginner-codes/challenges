# Challenge 751 - Decimal and Binary Palindromes

A number/string is a palindrome if the digits/characters are the same when read both forward and backward. Examples include `"racecar"` and `12321`. Given a positive number, check if the decimal or binary representation is a palindrome. 

Return the following:

- `"Decimal only."` if only the decimal representation is a palindrome.
- `"Binary only."` if only the binary representation is a palindrome.
- `"Decimal and binary."` if both are palindromes.
- `"Neither!"` if neither are palindromes.

## Examples
```python
palindrome_type(1306031) ➞ "Decimal only."
# decimal = 1306031
# binary  = "100111110110110101111"

palindrome_type(427787) ➞ "Binary only."
# decimal = 427787
# binary  = "1101000011100001011"

palindrome_type(313) ➞ "Decimal and binary."
# decimal = 313
# binary  = 100111001

palindrome_type(934) ➞ "Neither!"
# decimal = 934
# binary  = "1110100110"
```
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


def palindrome_type(number: int) -> str:
    return ""  # Put your code here!!!


test(751, palindrome_type)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            8337738
        ],
        "return": "Neither!"
    },
    {
        "args": [
            1306031
        ],
        "return": "Decimal only."
    },
    {
        "args": [
            4
        ],
        "return": "Decimal only."
    },
    {
        "args": [
            7115931
        ],
        "return": "Binary only."
    },
    {
        "args": [
            14441
        ],
        "return": "Decimal only."
    },
    {
        "args": [
            585585
        ],
        "return": "Decimal and binary."
    }
]
```

## Credits

Found on Edabit: [Decimal and Binary Palindromes](https://edabit.com/challenge/QuxCNBLcGJReCawjz)
