# Challenge 633 - Malthusian Catastrophe

A man named Thomas Malthus described what is now called a Malthusian Catastrophe. According to him, food production grows by a fixed amount, but population grows by a percentage. So, the food supply would soon be insufficient for the population.

Your job is to find out when that will occur. For this challenge, assume 1 population needs 1 unit of food production. Food production and population both start at 100. The year starts at 0.

The catastrophe happens when the population is larger than food production.

The function will be passed:

- `food_growth` — an integer — food production increase per year.
- `pop_mult` — a floating-point number — population growth multiplier per year.

## Examples
```python
malthusian(4255, 1.41) ➞ 20
# { food_prod: 85,200, pop: 96,467.77..., year: 20 }

malthusian(9433, 1.09) ➞ 107
# { food_prod: 1,009,431, pop: 1,010,730.28..., year: 107 }

malthusian(5879, 1.77) ➞ 12
# { food_prod: 70,648, pop: 94,553.84..., year: 12 }
```
## Notes

- Return the year that the overtake happens, not the next year.
- Make sure you don't make the mistake of adding a year, then calculating the changes to food and population. That way, you miss year 0.
- If the population and food production are equal, that is not a catastrophe.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def malthusian(food_growth: int, pop_mult: float) -> int:
    return 0  # Put your code here!!!


test(633, malthusian)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            3513,
            1.2
        ],
        "return": 40
    },
    {
        "args": [
            8194,
            1.12
        ],
        "return": 78
    },
    {
        "args": [
            6068,
            1.71
        ],
        "return": 13
    },
    {
        "args": [
            8381,
            1.8
        ],
        "return": 12
    },
    {
        "args": [
            1508,
            1.1
        ],
        "return": 74
    },
    {
        "args": [
            7139,
            1.1
        ],
        "return": 93
    },
    {
        "args": [
            6560,
            1.66
        ],
        "return": 14
    },
    {
        "args": [
            2214,
            1.53
        ],
        "return": 14
    },
    {
        "args": [
            7702,
            1.08
        ],
        "return": 119
    },
    {
        "args": [
            4859,
            1.87
        ],
        "return": 10
    }
]
```
## Credits

Found on Edabit: [Malthusian Catastrophe](https://edabit.com/challenge/zDei9LFWkX9d7wXyb)
