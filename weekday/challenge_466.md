# Challenge 466 - Total Sales of Product

In this question you will be given a table as below, where the first row lists the names of products, and each of row after that lists the sales of the product for each day (over some time range).
```python
[
  ["A", "B", "C"],
  [ 2 ,  7 ,  1 ],
  [ 3 ,  6 ,  6 ],
  [ 4 ,  5 ,  5 ]
]
```
Write a function that receives:

- A sales table as shown above.
- The name of a product.

The function should return the total sales if the product is in the list, otherwise return the string `"Product not found"`.

## Examples
```python
total_sales([
  ["A", "B", "C"],
  [ 2 ,  7 ,  1 ],
  [ 3 ,  6 ,  6 ],
  [ 4 ,  5 ,  5 ]
], "A") ➞ 9

# 2 + 3 + 4 = 9


total_sales([
  ["A", "B", "C"],
  [ 2 ,  7 ,  1 ],
  [ 3 ,  6 ,  6 ],
  [ 4 ,  5 ,  5 ]
], "C") ➞ 12

# 1 + 6 + 5 = 12


total_sales([
  ["A", "B", "C"],
  [ 2 ,  7 ,  1 ],
  [ 3 ,  6 ,  6 ],
  [ 4 ,  5 ,  5 ]
], "D") ➞ "Product not found"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def total_sales(table: list[list[str | int]], product: str) -> int | str:
    return 0  # Put your code here!!!


test(466, total_sales)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                [
                    "A",
                    "B",
                    "C"
                ],
                [
                    2,
                    7,
                    1
                ],
                [
                    3,
                    6,
                    6
                ],
                [
                    4,
                    5,
                    5
                ]
            ],
            "A"
        ],
        "return": 9
    },
    {
        "args": [
            [
                [
                    "A",
                    "B",
                    "C"
                ],
                [
                    2,
                    7,
                    1
                ],
                [
                    3,
                    6,
                    6
                ],
                [
                    4,
                    5,
                    5
                ]
            ],
            "B"
        ],
        "return": 18
    },
    {
        "args": [
            [
                [
                    "A",
                    "B",
                    "C"
                ],
                [
                    2,
                    7,
                    1
                ],
                [
                    3,
                    6,
                    6
                ],
                [
                    4,
                    5,
                    5
                ]
            ],
            "C"
        ],
        "return": 12
    },
    {
        "args": [
            [
                [
                    "A",
                    "B",
                    "C"
                ],
                [
                    2,
                    7,
                    1
                ],
                [
                    3,
                    6,
                    6
                ],
                [
                    4,
                    5,
                    5
                ]
            ],
            "D"
        ],
        "return": "Product not found"
    },
    {
        "args": [
            [
                [
                    "W",
                    "X",
                    "Y",
                    "Z"
                ],
                [
                    3,
                    5,
                    7,
                    1
                ],
                [
                    4,
                    5,
                    2,
                    3
                ]
            ],
            "A"
        ],
        "return": "Product not found"
    }
]
```
## Credits

Found on Edabit: [Total Sales of Product](https://edabit.com/challenge/kPKNb4c3QjCf5tHRM)
