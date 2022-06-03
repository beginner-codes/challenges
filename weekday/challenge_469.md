# Challenge 469 - Spicy Food

The facts are:

- You've just finished dinner.
- You love spicy food but your friend hates it.

Given your friend's unfortunate taste preferences, you decide to split the bill only for non-spicy items. You will pay in full for the spicy dishes.

Given two ordered lists, one classifying the dishes as spicy vs. non-spicy and the other listing their prices, write a function that outputs a list where the first element is how much you pay and the second element is how much your friend pays.

```python
bill_split(["S", "N", "S", "S"], [13, 18, 15, 4]) ➞ [41, 9]

# Since:
# You pay: [13, 9, 15, 4] = 41
# Friend pays: [0, 9, 0, 0] = 9
```
## Examples
```python
bill_split(["N", "S", "N"], [10, 10, 20]) ➞ [25, 15]
# You pay for half of both "N" dishes (5 + 10) and entirely pay for the "S" dish (10).

bill_split(["N", "N"], [10, 10]) ➞ [10, 10]

bill_split(["S", "N"], [41, 10]) ➞ [46, 5]
```
## Notes

- Remember to output a list in this order: `[your payment, friend's payment]`

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def bill_split(food: list[str], prices: list[int]) -> list[int, int]:
    return [0, 0]  # Put your code here!!!


test(469, bill_split)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "N",
                "S",
                "N"
            ],
            [
                10,
                10,
                20
            ]
        ],
        "return": [
            25,
            15
        ]
    },
    {
        "args": [
            [
                "N",
                "N"
            ],
            [
                10,
                10
            ]
        ],
        "return": [
            10,
            10
        ]
    },
    {
        "args": [
            [
                "S",
                "N"
            ],
            [
                41,
                10
            ]
        ],
        "return": [
            46,
            5
        ]
    },
    {
        "args": [
            [
                "S",
                "S",
                "S",
                "N",
                "N"
            ],
            [
                8,
                9,
                8,
                7,
                7
            ]
        ],
        "return": [
            32,
            7
        ]
    },
    {
        "args": [
            [
                "N",
                "N",
                "N",
                "S"
            ],
            [
                40,
                20,
                20,
                10
            ]
        ],
        "return": [
            50,
            40
        ]
    }
]
```
## Credits

Found on Edabit: [Spicy Food](https://edabit.com/challenge/KspbYHCtFZCcav7zx)
