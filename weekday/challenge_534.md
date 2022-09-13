# Challenge 534 - The Million Dollar Fence

Your task is to create a fence worth $1 million. You are given the price of the material (per character), meaning the length of the fence will change depending on the cost of the material.

Create a function which constructs this pricey pricey fence, using the letter "H" to build.
```python
construct_fence("$50,000") ➞ "HHHHHHHHHHHHHHHHHHHHHHHHHHHH"
# 20 fence posts were set up ($1,000,000 / $50,000 = 20)
```
## Examples
```python
construct_fence("$50,000") ➞ "HHHHHHHHHHHHHHHHHHHHHHHHHHHH"

construct_fence("$100,000") ➞ "HHHHHHHHHH"

construct_fence("$1,000,000") ➞ "H"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def construct_fence(cost: str) -> str:
    return "" # Put your code here!!!


test(534, construct_fence)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "$10,000"
        ],
        "return": "HHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHH"
    },
    {
        "args": [
            "$100,000"
        ],
        "return": "HHHHHHHHHH"
    },
    {
        "args": [
            "$1,000,000"
        ],
        "return": "H"
    },
    {
        "args": [
            "$20,000"
        ],
        "return": "HHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHHH"
    },
    {
        "args": [
            "$50,000"
        ],
        "return": "HHHHHHHHHHHHHHHHHHHH"
    }
]
```
## Credits

Found on Edabit: [The Million Dollar Fence](https://edabit.com/challenge/XqxeeB4nYpS53noTA)
