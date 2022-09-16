# Challenge 537 - Pages in a Book

Suppose that you add up all of the page numbers in a book. If the total is 21, the book could only have 6 pages because `1 + 2 + 3 + 4 + 5 + 6 = 21`. If the total were 25, that would be impossible because the next number in the series is 28 (`21 + 7`).

Create a function that, given the total sum of the pages as an argument, returns `True` if it is a valid total and `False` if it is not.

Can you devise a solution that is more efficient than simply adding consecutive integers as I did above?

## Examples
```python
pages_in_book(5) ➞ False

pages_in_book(4005) ➞ True

pages_in_book(9453) ➞ True
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def pages_in_book(page_sum: int) -> bool:
    return False # Put your code here!!!


test(537, pages_in_book)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            125250
        ],
        "return": true
    },
    {
        "args": [
            9474
        ],
        "return": false
    },
    {
        "args": [
            4005
        ],
        "return": true
    },
    {
        "args": [
            920046
        ],
        "return": true
    },
    {
        "args": [
            9453
        ],
        "return": true
    }
]
```
## Credits

Found on Edabit: [Pages in a Book](https://edabit.com/challenge/nugyAtjRNQPTHLJNR)
