# Challenge 732 - Binary to ASCII Conversion

Create a function that takes a string of 1's and 0's as an argument and return the equivalent decoded ASCII text.
Characters can be in the range of `"00000000"` to `"11111111"`, which means every eight digits of binary input
represents a single character.

```python
a = 01100001
b = 01100010
c = 01100011
```

If you were to combine these characters into the string `"abc"`, the corresponding binary would
be `011000010110001001100011`.

## Examples

```python
binary_conversion("0110001001100101011001110110100101101110011011100110010101110010") ➞ "beginner"

binary_conversion("001100010011001000110011") ➞ "123"

binary_conversion("010010000110010101101100011011000110111100111111") ➞ "Hello?"
```

## Notes

- If you are given an empty string as input, you must also return an empty string. Otherwise, the input will always be a
  valid binary string.

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


def binary_conversion(binary: str) -> str:
    return ""  # Put your code here!!!


test(732, binary_conversion)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
  {
    "args": [
      ""
    ],
    "return": ""
  },
  {
    "args": [
      "0110001001100101011001110110100101101110011011100110010101110010"
    ],
    "return": "beginner"
  },
  {
    "args": [
      "0010000101000000001000110010010000100101010111100010011000101010001010000010100101010001010101110100010101110010011101000111100101010101010010010100111101001100011001000110011001100111011000100110001001101000011011100110110101001001010010110100001001001010010010110100100001001001010101010100111100101000001111110011111000111111001111000111111001111110011111100111111001111110001010010010100000101010001001100010010101011110001110010011100000110111001100010011001100101111001011010010111100101010001011010010101000101111"
    ],
    "return": "!@#$%^&*()QWErtyUIOLdfgbbhnmIKBJKHIUO(?>?<~~~~~)(*&%^98713/-/*-*/"
  },
  {
    "args": [
      "001100010011001000110011"
    ],
    "return": "123"
  },
  {
    "args": [
      "010010000110010101101100011011000110111100111111"
    ],
    "return": "Hello?"
  }
]
```

## Credits

Found on Edabit: [Binary to ASCII Conversion](https://edabit.com/challenge/Wm8Zin8gQGsupNmbJ)
