# Challenge 788 - The Major Sum

Create a function that takes an integer list and return the biggest between the positive sum, negative sum, or the number of 0`s. The major is understood as the greatest absolute value of the three.

For `[1,2,3,4,0,0,-3,-2]` the function has to return 10, because:

- Positive sum = `1+2+3+4 = 10`
- Negative sum = `(-3)+(-2) = -5`
- 0s count = `2 (there are two zeros in list)`

## Examples
```python
major_sum([1, 2, 3, 4, 0, 0, -3, -2]) ➞ 10

major_sum([-4, -8, -12, -3, 4, 7, 1, 3, 0, 0, 0, 0]) ➞ -27

major_sum([0, 0, 0, 0, 0, 1, 2, -3]) ➞ 5
# Because -3 < 1+2 < 0sCount = 5
```
## Notes

- All numbers are integers.
- There aren't empty lists.

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


def major_sum(numbers: list[int]) -> int:
    return 0  # Put your code here!!!


test(788, major_sum)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                1
            ]
        ],
        "return": 1
    },
    {
        "args": [
            [
                1,
                2,
                3,
                4,
                -5,
                -4,
                -3,
                -2,
                -1,
                0
            ]
        ],
        "return": -15
    },
    {
        "args": [
            [
                -1
            ]
        ],
        "return": -1
    },
    {
        "args": [
            [
                2,
                0,
                -1
            ]
        ],
        "return": 2
    },
    {
        "args": [
            [
                0,
                0,
                0,
                0,
                0,
                1,
                2,
                -3
            ]
        ],
        "return": 5
    }
]
```

## Credits

Found on Edabit: [The Major Sum](https://edabit.com/challenge/kiX7WjSFeTmBYcEgK)
