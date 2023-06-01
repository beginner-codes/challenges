# Challenge 675 - Got Enough Money?

Create a function that returns any of the items you can afford in the store with the money you have in your wallet. Sort the list in alphabetical order.

## Examples
```python
items_purchase({
  "Water": "$1",
  "Bread": "$3",
  "TV": "$1,000",
  "Fertilizer": "$20"
}, "$300") ➞ ["Bread", "Fertilizer", "Water"]

items_purchase({
  "Apple": "$4",
  "Honey": "$3",
  "Fan": "$14",
  "Bananas": "$4",
  "Pan": "$100",
  "Spoon": "$2"
  }, "$100") ➞ ["Apple", "Bananas", "Fan", "Honey", "Pan", "Spoon"]

items_purchase({
  "Phone": "$999",
  "Speakers": "$300",
  "Laptop": "$5,000",
  "PC": "$1200"},
"$1") ➞ "Nothing"
```
## Notes

- Return `"Nothing"` if you can't afford anything from the store.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test

    
def items_purchase(products: dict[str, str]) -> list[str] | str:
    return ""  # Put your code here!!!


test(675, items_purchase)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            {
                "Apple": "$4",
                "Honey": "$3",
                "Fan": "$14",
                "Bananas": "$4",
                "Pan": "$100",
                "Spoon": "$2"
            },
            "$100"
        ],
        "return": [
            "Apple",
            "Bananas",
            "Fan",
            "Honey",
            "Pan",
            "Spoon"
        ]
    },
    {
        "args": [
            {
                "Phone": "$999",
                "Speakers": "$300",
                "Laptop": "$5,000",
                "PC": "$1200"
            },
            "$1"
        ],
        "return": "Nothing"
    },
    {
        "args": [
            {
                "Water": "$1",
                "Bread": "$3",
                "TV": "$1,000",
                "Fertilizer": "$20"
            },
            "$300"
        ],
        "return": [
            "Bread",
            "Fertilizer",
            "Water"
        ]
    }
]
```
## Credits

Found on Edabit: [Got Enough Money?](https://edabit.com/challenge/9ZAk3EEoQ9YPGGYhA)
