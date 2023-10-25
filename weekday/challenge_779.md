# Challenge 779 - Binary Tree Nodes

We have a nodes list and parents list, where nodes list represents the value of each node in a Binary Tree, and the parents list is the parent of each corresponding node from the node list.
```
Node    Parent
1       2
3       2
6       8
9       8
2       5
8       5
5       -1
```
Write a function that is given a node list, parents list, and a node value. The function should return the type of node that has the given value: one of "Root", "Leaf", "Inner", or "Doesn't Exist".

- Root: If the node has no parent (-1 parent value).
- Leaf: If the node has a parent but no children.
- Inner: If the node has children and a parent.
- Doesn't exist: If no node in the tree has a corresponding value.

## Examples
```python
node_type([1, 3, 6, 9, 2, 8, 5], [2, 2, 8, 8, 5, 5, -1], 5) ➞ "Root"

node_type([1, 3, 6, 9, 2, 8, 5], [2, 2, 8, 8, 5, 5, -1], 6) ➞ "Leaf"

node_type([1, 3, 6, 9, 2, 8, 5], [2, 2, 8, 8, 5, 5, -1], 2) ➞ "Inner"

node_type([1, 3, 6, 9, 2, 8, 5], [2, 2, 8, 8, 5, 5, -1], 10) ➞ "Doesn't exist"
```
## Notes

- All values of node list are unique.

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


def node_type(node_values: list[int], node_parents: list[int], node_value: int) -> str:
    return ""  # Put your code here!!!


test(779, node_type)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                5,
                6,
                8,
                7,
                1,
                9,
                4,
                11,
                10,
                2
            ],
            [
                8,
                8,
                -1,
                8,
                7,
                4,
                5,
                4,
                1,
                1
            ],
            11
        ],
        "return": "Leaf"
    },
    {
        "args": [
            [
                1,
                3,
                6,
                9,
                2,
                8,
                5
            ],
            [
                2,
                2,
                8,
                8,
                5,
                5,
                -1
            ],
            1
        ],
        "return": "Leaf"
    },
    {
        "args": [
            [
                1,
                3,
                6,
                9,
                2,
                8,
                5
            ],
            [
                2,
                2,
                8,
                8,
                5,
                5,
                -1
            ],
            9
        ],
        "return": "Leaf"
    },
    {
        "args": [
            [
                6,
                3,
                1,
                2,
                5,
                7,
                4,
                6,
                8
            ],
            [
                3,
                1,
                6,
                1,
                2,
                3,
                8,
                -1,
                6
            ],
            5
        ],
        "return": "Leaf"
    },
    {
        "args": [
            [
                1,
                3,
                6,
                9,
                2,
                8,
                5
            ],
            [
                2,
                2,
                8,
                8,
                5,
                5,
                -1
            ],
            5
        ],
        "return": "Root"
    }
]

```

## Credits

Found on Edabit: [Binary Tree Nodes](https://edabit.com/challenge/Cp3JRpooAqfA4kGkv)
