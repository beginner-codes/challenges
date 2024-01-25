# Challenge 811 - Shorthand for Key Signatures

Given a string containing a key signature written in shorthand, create a function which replaces the shorthand with its full written name.

- A lowercase letter denotes a minor key.
- An uppercase letter denotes a major key.

See the examples below for a more helpful guide!

## Examples
```python
full_key_name("Prelude in C") ➞ "Prelude in C major"

full_key_name("Fugue in c") ➞ "Fugue in C minor"

full_key_name("Toccata and Fugue in d") ➞ "Toccata and Fugue in D minor"

full_key_name("Sonata in eb") ➞ "Sonata in Eb minor"
```
## Notes

- Write the letter name in uppercase (ignore b and #).
- Write "major" or "minor" in all lowercase (rather than "Major" or "Minor").

## Hint

The first letter of the term should always be capital, even if it's "b".

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


def full_key_name(shorthand: str) -> str:
    return ""  # Put your code here!!!


test(811, full_key_name)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "Opera in f"
        ],
        "return": "Opera in F minor"
    },
    {
        "args": [
            "Fugue in g"
        ],
        "return": "Fugue in G minor"
    },
    {
        "args": [
            "Fugue in G"
        ],
        "return": "Fugue in G major"
    },
    {
        "args": [
            "Prelude in Eb"
        ],
        "return": "Prelude in Eb major"
    },
    {
        "args": [
            "Mass in c"
        ],
        "return": "Mass in C minor"
    }
]
```

## Credits

Found on Edabit: [Shorthand for Key Signatures](https://edabit.com/challenge/yqeCTqSemWx5rJ7LZ)
