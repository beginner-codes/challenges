# Challenge 774 - Maximum Travel Distance

Write a function that takes fuel (liters), fuel_usage (liters/100km), passengers, state of air conditioning and returns the maximum distance that the car can travel.

- Fuel is the number of liters of fuel in the fuel tank.
- Fuel usage is **basic** fuel consumption per 100km (with the driver inside only).
- Every additional passenger is increasing basic fuel consumption by 5%.
- If the air conditioner is ON (`True`), its increasing total (not basic) fuel consumption by 10%.

## Examples
```python
total_distance(70.0, 7.0, 0, False) ➞ 1000.0

total_distance(36.1, 8.6, 3, True) ➞ 331.8

total_distance(55.5, 5.5, 5, false) ➞ 807.3
```
## Notes

- The fuel and fuel usage are always greater than 1
- There are always 0 or more passengers
- Round your answer to the nearest tenth

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


def total_distance(fuel: float, fuel_usage: float, passengers: int, ac_on: bool) -> float:
    return 0.0  # Put your code here!!!


test(774, total_distance)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            11.0,
            11.0,
            0,
            false
        ],
        "return": 100.0
    },
    {
        "args": [
            36.1,
            8.6,
            3,
            true
        ],
        "return": 331.8
    },
    {
        "args": [
            30.0,
            3.0,
            0,
            false
        ],
        "return": 1000.0
    },
    {
        "args": [
            300.0,
            25.0,
            11,
            true
        ],
        "return": 703.8
    },
    {
        "args": [
            50.0,
            7.0,
            3,
            true
        ],
        "return": 564.7
    }
]
```

## Credits

Found on Edabit: [Maximum Travel Distance](https://edabit.com/challenge/FjiriGn8gc5RE8Xm2)
