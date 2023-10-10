# Challenge 768 - Combinatorial Exploration

Given a known number of unique items, how many ways could we arrange them in a row?

Create a function that takes an integer and returns the number of digits of the number of possible permutations for n768 unique items. For instance, 5 unique items could be arranged in 120 unique ways. 120 has 3 digits, hence the integer 3 is returned.

## Examples
```python
num_permutation_digits(0) ➞ 1

num_permutation_digits(1) ➞ 1

num_permutation_digits(5) ➞ 3

num_permutation_digits(8) ➞ 5
```
## Notes

- This challenge requires some understanding of combinatorics.

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


def num_permutation_digits(num_items: int) -> int:
    return 0  # Put your code here!!!


test(768, num_permutation_digits)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            10
        ],
        "return": 7
    },
    {
        "args": [
            15
        ],
        "return": 13
    },
    {
        "args": [
            2
        ],
        "return": 1
    },
    {
        "args": [
            19
        ],
        "return": 18
    },
    {
        "args": [
            16
        ],
        "return": 14
    }
]
```

## Credits

Found on Edabit: [Combinatorial Exploration](https://edabit.com/challenge/oQ99uE4iPNbEnf9QZ)
