# Challenge 749 - A Simple Comparison

You're give a list of numbers and a second list that should contain the squared values of the numbers from the first list.

Create a function which takes these two lists and returns `True` if all squared values are found in the second list, `False` otherwise.
```python
lst1 = [121, 144, 19, 161, 19, 144, 19, 11]  
lst2 = [121, 14641, 20736, 361, 25921, 361, 20736, 361]
```
Returns `True` because 121 is square of 11, 14641 is square of 121, 20736 is square of 144, 361 is square of 19, 25921 the square of 161, and so on...
```python
lst1 = [121, 144, 19, 161, 19, 144, 19, 11] 
lst2 = [11*11, 121*121, 144*144, 19*19, 161*161, 19*19, 144*144, 19*19]
```
## Examples
```python
simple_comp([121, 144, 19, 161, 19, 144, 19, 11], [121, 14641, 20736, 361, 25921, 361, 20736, 361]) ➞ True

simple_comp([4, 4], [1, 31]) ➞ False

simple_comp([2, 2, 3], [4, 4, 9]) ➞ True
```
## Notes

- Numbers can be in any order.

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


def simple_comp(list_1: list[int], list_2: list[int]) -> bool:
    return False  # Put your code here!!!


test(749, simple_comp)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            null,
            []
        ],
        "return": false
    },
    {
        "args": [
            [
                10000000,
                100000000
            ],
            [
                100000000000000,
                10000000000000000
            ]
        ],
        "return": true
    },
    {
        "args": [
            [
                121,
                144,
                19,
                161,
                19,
                144,
                19,
                11,
                1008
            ],
            [
                121,
                14641,
                20736,
                36100,
                25921,
                361,
                20736,
                361
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                2,
                2,
                3
            ],
            [
                4,
                9,
                9
            ]
        ],
        "return": false
    },
    {
        "args": [
            [
                -121,
                -144,
                19,
                -161,
                19,
                -144,
                19,
                -11
            ],
            [
                121,
                14641,
                20736,
                361,
                25921,
                361,
                20736,
                361
            ]
        ],
        "return": true
    }
]
```

## Credits

Found on Edabit: [A Simple Comparison](https://edabit.com/challenge/YXjx9G5uQ4CdYPuB4)
