# Challenge 690 - Safecracker

Traditional safes use a three-wheel locking mechanism, with the safe combination entered using a dial on the door of the safe. The dial is marked with clockwise increments between 0 and 99. The three-number combination is entered by first dialling to the right (clockwise), then to the left (anti-clockwise), and then to the right (clockwise) again. Combination numbers are read from the top of the dial.

Given the starting (top) position of the dial and the increments used for each turn of the dial, return a list containing the combination of the safe.

Step-By-Step Example
```python
safecracker(0, [3, 10, 5]) ➞ [97, 7, 2]
```
Starting dial position of 0 (same as the diagram above).

First turn (rightward) of 3 increments:
```
0 -> 99, 98, 97
```
First number of combination = 97

Second turn (leftward) of 10 increments:
```
97 -> 98, 99, 0, 1, 2, 3, 4, 5, 6, 7
```
Second number of combination = 7

Third turn (rightward) of 5 increments:
```
7 -> 6, 5, 4, 3, 2
```
Third number of combination = 2

The final combination is [97, 7, 2]

## Other Examples
```python
safecracker(96, [54, 48, 77]) ➞ [42, 90, 13]

safecracker(43, [51, 38, 46]) ➞ [92, 30, 84]

safecracker(4, [69, 88, 55]) ➞ [35, 23, 68]
```
## Notes

- Each of the three combination numbers will be different.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def safecracker(starting_position: int, increments: list[int]) -> list[int]:
    return []  # Put your code here!!!


test(690, safecracker)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            85,
            [
                25,
                24,
                73
            ]
        ],
        "return": [
            60,
            84,
            11
        ]
    },
    {
        "args": [
            77,
            [
                73,
                98,
                55
            ]
        ],
        "return": [
            4,
            2,
            47
        ]
    },
    {
        "args": [
            45,
            [
                63,
                96,
                30
            ]
        ],
        "return": [
            82,
            78,
            48
        ]
    },
    {
        "args": [
            0,
            [
                21,
                94,
                92
            ]
        ],
        "return": [
            79,
            73,
            81
        ]
    },
    {
        "args": [
            67,
            [
                71,
                93,
                93
            ]
        ],
        "return": [
            96,
            89,
            96
        ]
    }
]
```
## Credits

Found on Edabit: [Safecracker](https://edabit.com/challenge/7RrPMoWifqRHPPqj2)
