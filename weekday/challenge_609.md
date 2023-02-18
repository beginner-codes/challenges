# Challenge 609 - Early Birds

A Natural Number String Sequence is a string containing all numbers, starting from `0`, joined without spaces or other delimiters between them.
```python
"01234567891011121314151617181920..."
```
If you think of the sequence as a list, any number has a natural position index it occupies within a string long enough to contain it based on the real position in the numeric sequence. Looking at the example above, numbers from `0` to `9` are equals to their index position in the string; starting from `10`, every number has a string natural index position different from itself (number `10` has a position of `10|11` because it has two digits, number `11` has a position of `12|13`, and so on).

Any number that appears in the sequence before its natural position is an "Early Bird." Suppose that we want to know if number `12` is an "Early Bird" in the above example sequence:
```
01234567891011121314151617181920
_!!___________!!________________
```
Natural position index of `12` is `|14, 15|` (after `11` and before `13` in the numeric sequence), but, if we look closely at the sequence, it appears before its natural position, at index `|1, 2|` (after `0` and before `3`): `12` is then an "Early Bird" number (and the first to appear).

You are given two integers as parameters: the ending number of the string sequence to generate, and the number to analyze. You must implement a function that returns a list that contains the position indexes of the number (with every position index being a list in turn), and the string `"Early Bird!"` as the last element of the list only if the number is an "Early Bird." If the number is not an "Early Bird" just return its natural position index.

## Examples
```python
is_early_bird(20, 14) ➞ [[18, 19]]

is_early_bird(20, 12) ➞ [[1, 2], [14, 15], "Early Bird!"]

is_early_bird(101, 101) ➞ [[10, 11, 12], [193, 194, 195], "Early Bird!"]
```
## Notes

- The given number will be greater than 9 for every case, as trivially every single-digit number appears at the same index in the numeric sequence and in the string sequence.
- The position indexes have to be in the order they appear in the string sequence.
- The string at the end of the list has to be present only if n is an Early Bird.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def is_early_bird(end: int, number: int) -> list[list | str]:
    return []  # Put your code here!!!


test(609, is_early_bird)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            50,
            34
        ],
        "return": [
            [
                3,
                4
            ],
            [
                58,
                59
            ],
            [
                77,
                78
            ],
            "Early Bird!"
        ]
    },
    {
        "args": [
            900,
            888
        ],
        "return": [
            [
                166,
                167,
                168
            ],
            [
                2554,
                2555,
                2556
            ],
            [
                2555,
                2556,
                2557
            ],
            [
                2556,
                2557,
                2558
            ],
            "Early Bird!"
        ]
    },
    {
        "args": [
            2000,
            666
        ],
        "return": [
            [
                122,
                123,
                124
            ],
            [
                1888,
                1889,
                1890
            ],
            [
                1889,
                1890,
                1891
            ],
            [
                1890,
                1891,
                1892
            ],
            [
                5555,
                5556,
                5557
            ],
            "Early Bird!"
        ]
    },
    {
        "args": [
            20,
            12
        ],
        "return": [
            [
                1,
                2
            ],
            [
                14,
                15
            ],
            "Early Bird!"
        ]
    },
    {
        "args": [
            400,
            240
        ],
        "return": [
            [
                610,
                611,
                612
            ]
        ]
    }
]
```
## Credits

Found on Edabit: [Early Birds](https://edabit.com/challenge/hCAStny5sJwYP3evS)
