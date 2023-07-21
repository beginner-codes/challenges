# Challenge 710 - Pentagonal Number

Write a function that takes a positive integer and calculates how many dots exist in a pentagonal shape around the center dot on the Nth iteration.

In the diagram below you can see the first iteration is only a single dot. On the second, there are 6 dots. On the third, there are 16 dots, and on the fourth there are 31 dots.

```
 •     •           •                   • 
     • · •      •  ·  •            •   ·   •
      • •     •  · · ·  •       •   ·  ·  ·   •
               •  · ·  •     •   ·   · · ·   ·   • 
                •  •  •       •   ·   · ·   ·   •
                               •   ·   ·   ·   •
                                •   •    •    •
```

Return the number of dots that exist in the whole pentagon on the Nth iteration.

## Examples
```python
pentagonal(1) ➞ 1

pentagonal(2) ➞ 6

pentagonal(3) ➞ 16

pentagonal(8) ➞ 141
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def pentagonal(iterations: int) -> int:
    return 0  # Put your code here!!!


test(710, pentagonal)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            10
        ],
        "return": 226
    },
    {
        "args": [
            13
        ],
        "return": 391
    },
    {
        "args": [
            62
        ],
        "return": 9456
    },
    {
        "args": [
            8
        ],
        "return": 141
    },
    {
        "args": [
            50
        ],
        "return": 6126
    }
]
```
## Credits

Found on Edabit: [Pentagonal Number](https://edabit.com/challenge/st8mDxreMcuWxuz8c)
