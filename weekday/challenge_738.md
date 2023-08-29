# Challenge 738 - Vowel to Vowel Links

Given a sentence, return `True` if any two adjacent words have this property: One word ends with a vowel while the
word immediately after also begins with a vowel.

## Examples

```python
vowel_links("a very large appliance") ➞ True

vowel_links("an open fire") ➞ False

vowel_links("a sudden applause") ➞ False
```

## Notes

- You can expect sentences in only lowercase, with no punctuation.

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


def vowel_links(sentence: str) -> bool:
    return False  # Put your code here!!!


test(738, vowel_links)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
  {
    "args": [
      "the eagle swooped down low"
    ],
    "return": true
  },
  {
    "args": [
      "beneficial luggage"
    ],
    "return": false
  },
  {
    "args": [
      "creative environment"
    ],
    "return": true
  },
  {
    "args": [
      "this is not a drill"
    ],
    "return": false
  },
  {
    "args": [
      "the large appliances"
    ],
    "return": true
  }
]
```

## Credits

Found on Edabit: [Vowel to Vowel Links](https://edabit.com/challenge/PxxZprxCjDrzaTcLQ)
