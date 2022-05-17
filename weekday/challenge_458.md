# Challenge 458 - N Differences

Write a function that transforms an array into an array of its differences repeatedly until there exists only one element left. A difference is `A[n+1] - A[n]`.

To illustrate:
```python
[5, 1, 9, 3, 4, 0]

[-4, 8, -6, 1, -4]
# 1 - 5 = -4; 9 - 1 = 8; 3 - 9 = -6; etc.

[12, -14, 7, -5]

[-26, 21, -12]

[47, -33]

-80 
```
## Examples
```python
n_differences([5, 1, 9, 3, 4, 0]) ➞ -80

n_differences([1, 1, 1, 1]) ➞ 0

n_differences([5, 8, 8]) ➞ -3
```
## Notes

- Each array will have at least two elements.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def n_differences(array: list[int]) -> int:
    return 0  # Put your code here!!!


test(448, n_differences)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                5,
                1,
                9,
                3,
                4,
                0
            ]
        ],
        "return": -80
    },
    {
        "args": [
            [
                8,
                9,
                2,
                5,
                4,
                3,
                3,
                1,
                6
            ]
        ],
        "return": -94
    },
    {
        "args": [
            [
                5,
                1,
                9,
                6,
                1,
                7,
                3,
                4
            ]
        ],
        "return": 118
    },
    {
        "args": [
            [
                1,
                1,
                1,
                1
            ]
        ],
        "return": 0
    },
    {
        "args": [
            [
                5,
                9,
                7,
                3
            ]
        ],
        "return": 4
    },
    {
        "args": [
            [
                1,
                5,
                3,
                9,
                7
            ]
        ],
        "return": -30
    },
    {
        "args": [
            [
                5,
                8,
                8
            ]
        ],
        "return": -3
    },
    {
        "args": [
            [
                4,
                0,
                0,
                0,
                1
            ]
        ],
        "return": 5
    },
    {
        "args": [
            [
                3,
                5
            ]
        ],
        "return": 2
    }
]
```
## Credits

Found on Edabit: [N Differences](https://edabit.com/challenge/J7HPbiP9WRTCteazx)
