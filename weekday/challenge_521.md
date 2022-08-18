# Challenge 521 - Numerical Morphisms 

A number, that elevated to the power of another number "ends" with the same num, is automorphic.
```python
5² = 25
# It's automorphic because "25" ends with "5"

5³  = 125
# It's automorphic because "125" ends with "5"

76⁴ = 33362176
# It's automorphic because "33362176" ends with "76"
```
A number can have various powers that make it automorphic (i.e. look at number 5 in the above example). In this challenge, you have to verify if the given number is automorphic for each power from 2 up to 10.

Given a non-negative integer num, implement a function that returns the string:

- `"Polymorphic"` if num is automorphic for every power from 2 up to 10.
- `"Quadrimorphic"` if num is automorphic for only four powers (any from 2 up to 10).
- `"Dimorphic"` if num is automorphic for only two powers (any from 2 up to 10).
- `"Enamorphic"` if num is automorphic for only one power (any from 2 up to 10).
- `"Amorphic"` if num is not automorphic for any powers from 2 up to 10.

## Examples
```python
power_morphic(5) ➞ "Polymorphic"
# From 2 up to 10, every power of 5 ends with 5

power_morphic(21) ➞ "Enamorphic"
# 21⁶ = 85766121

power_morphic(7) ➞ "Dimorphic"
# 7⁵ = 716807
# 7⁹ = 40353607

power_morphic(4) ➞ "Quadrimorphic"
# 4³ = 64
# 4⁵ = 1024
# 4⁷ = 16384
# 4⁹ = 262144

power_morphic(10) ➞ "Amorphic"
# There are no powers that make it automorphic
```
## Notes

- You can do a complete loop cycle to check if num is automorphic for each power, or you can try to spot the discriminants that permit you to shorten the logic of your code.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def power_morphic(number: int) -> str:
    return "" # Put your code here!!!


test(521, power_morphic)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            1
        ],
        "return": "Polymorphic"
    },
    {
        "args": [
            10
        ],
        "return": "Amorphic"
    },
    {
        "args": [
            7
        ],
        "return": "Dimorphic"
    },
    {
        "args": [
            625
        ],
        "return": "Polymorphic"
    },
    {
        "args": [
            9376
        ],
        "return": "Polymorphic"
    },
    {
        "args": [
            9999
        ],
        "return": "Quadrimorphic"
    },
    {
        "args": [
            121
        ],
        "return": "Amorphic"
    },
    {
        "args": [
            501
        ],
        "return": "Quadrimorphic"
    },
    {
        "args": [
            2030
        ],
        "return": "Amorphic"
    },
    {
        "args": [
            3376
        ],
        "return": "Enamorphic"
    }
]
```
## Credits

Found on Edabit: [Numerical Morphisms](https://edabit.com/challenge/RqhLJk82ySnmxxJBi)
