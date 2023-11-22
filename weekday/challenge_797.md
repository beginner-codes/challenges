# Challenge 797 - Plant Trees

We need your help to plant some trees. You are given three parameters:

- width of the land
- length of the land
- gap between the trees

You have to create an algorithm to return the number of trees which can be planted on the edges of the given land in a symmetrical layout as shown below (non-symmetrical gap = x, tree = o, gap = -):
```python
w=3, l=3, gap=1
plant_trees(w, l, gap) ➞ 4

o - o
-   -
o - o

# You can plant 4 trees.

w=3, l=3, gap=3
plant_trees(w, l, gap) ➞ 2

o - -
-   -
- - o

# You can plant 2 trees.
```
If the layout is not symmetrical, you have to return 0:
```python
w=3, l=3, gap=2
plant_trees(w, l, gap) ➞ 0

o - -
x   o
x x x

# Planting 2 trees mean the gap of two trees will be greater than 2.

o - -
x   o
o - -

# Planting 3 trees mean the gap of two trees will be less than 2.
```
Another Example for better understanding:
```python
w=3, l=3, gap=0
plant_trees(w, l, gap) ➞ 8

o o o
o   o
o o o

# You can plant 8 trees.
```
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


def plant_trees(width: int, height: int, gap: int) -> int:
    return 0  # Put your code here!!!


test(797, plant_trees)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            3,
            3,
            0
        ],
        "return": 8
    },
    {
        "args": [
            3,
            3,
            1
        ],
        "return": 4
    },
    {
        "args": [
            7,
            7,
            3
        ],
        "return": 6
    },
    {
        "args": [
            3,
            3,
            10
        ],
        "return": 0
    },
    {
        "args": [
            3,
            3,
            2
        ],
        "return": 0
    },
    {
        "args": [
            3,
            3,
            3
        ],
        "return": 2
    }
]
```

## Credits

Found on Edabit: [Plant Trees 🌲](https://edabit.com/challenge/RzrKedEonc3BJGhY5)
