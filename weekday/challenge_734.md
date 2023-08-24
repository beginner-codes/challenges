# Challenge 734 - Simple Symbols

Create a function that takes a string and determine if it's a valid sequence by either returning `True` or `False`. The
string will be composed of `+` and `=` symbols with several characters between them (e.g. `"++d+===+c++==a"`) and for
the string to be `True`, each letter must be surrounded by a `+` symbol. So the string would be `False`.

## Examples

```python
simple_symbols("f++d+") ➞ False

simple_symbols("+d+=3=+s+") ➞ True

simple_symbols("==+p+++++++++====8+z++++") ➞ True
```

## Notes

- The given string will not be empty and will have at least one letter.

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


def simple_symbols(string: str) -> bool:
    return False  # Put your code here!!!


test(734, simple_symbols)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
  {
    "args": [
      "======2+++4+u===+i+"
    ],
    "return": false
  },
  {
    "args": [
      "+u+====3+mmmmm===m++"
    ],
    "return": false
  },
  {
    "args": [
      "+d+=3=+s+"
    ],
    "return": true
  },
  {
    "args": [
      "==+p+++++++++====8+z++++"
    ],
    "return": true
  },
  {
    "args": [
      "f++d+"
    ],
    "return": false
  }
]
```

## Credits

Found on Edabit: [Simple Symbols](https://edabit.com/challenge/64w3Mpumi7kTA82Sv)
