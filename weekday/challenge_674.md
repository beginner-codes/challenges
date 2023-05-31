# Challenge 674 - Valid Prices

There has been a masterdata issue which affected the prices of some products. Check if each product has a valid price (integer or float, and greater than or equal to zero). Products with a price of 0 are free and count as a valid price.

The return value should be true or false.

## Examples
```python
has_valid_price({ "product": "Milk", "price": 1.50 }) ➞ True

has_valid_price({ "product": "Cheese", "price": -1 }) ➞ False

has_valid_price({ "product": "Eggs", "price": 0 }) ➞ True

has_valid_price({ "product": "Cereals", "price": "3.0" }) ➞ False

has_valid_price(None) ➞ False
```
## Notes

- Type of the price should be an integer or float. If it's anything else, you should return `False`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def has_valid_price(product: dict[str, str | int | float | None] | None) -> bool:
    return False  # Put your code here!!!


test(674, has_valid_price)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            {
                "product": "Milk",
                "price": 1.5
            }
        ],
        "return": true
    },
    {
        "args": [
            null
        ],
        "return": false
    },
    {
        "args": [
            {
                "product": "Beer",
                "price": null
            }
        ],
        "return": false
    },
    {
        "args": [
            {
                "product": "Eggs",
                "price": 0
            }
        ],
        "return": true
    },
    {
        "args": [
            {
                "product": "Flour"
            }
        ],
        "return": false
    }
]
```
## Credits

Found on Edabit: [Find the Bugs: Returning Valid Prices](https://edabit.com/challenge/bTQyk8xSumqLSzeXX)
