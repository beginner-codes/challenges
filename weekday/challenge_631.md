# Challenge 631 - Radioactive Decay

A half life is the amount of time for half of a radioactive substance to decay.

After 1 half life, 50% of a substance will be left.
After 2 half lives, 25% of a substance will be left.
After 3 half lives, 12.5% of a substance will be left, etc...

Create a function which calculates the remaining mass and the number of years that it took for the substance to decay. You will be given:

- The mass of the substance.
- The time in years for a half life to elapse.
- The number of half lives.

## Worked Example
```python
halflife_calculator(1000, 5730, 2) ➞ [250, 11460]

# There are 2 half lives, so the mass decays from 1000 to 500, then from 500 to 250.
# Each halflife is 5730 years, and since there were 2, it took 11460 years in total.
```
## Examples
```python
half_life_calculator(1600, 6, 3) ➞ [200, 18]

half_life_calculator(13, 500, 1) ➞ [6.5, 500]

half_life_calculator(100, 35, 5) ➞ [3.125, 175]
```
## Notes

- Round the final mass to three decimal places.
- All inputs are positive numbers.
- Return the final mass first, then the number of years.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def half_life_calculator(mass: int, half_life: int, elapsed_half_lives: int) -> list[float | int]:
    return []  # Put your code here!!!


test(631, half_life_calculator)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            100,
            35,
            5
        ],
        "return": [
            3.125,
            175
        ]
    },
    {
        "args": [
            1600,
            6,
            3
        ],
        "return": [
            200,
            18
        ]
    },
    {
        "args": [
            1000,
            5730,
            2
        ],
        "return": [
            250,
            11460
        ]
    },
    {
        "args": [
            13,
            500,
            1
        ],
        "return": [
            6.5,
            500
        ]
    },
    {
        "args": [
            11037,
            53,
            6
        ],
        "return": [
            172.453,
            318
        ]
    }
]
```
## Credits

Found on Edabit: [Radioactive Decay](https://edabit.com/challenge/wtBko8Bc8o8Tmra3q)
