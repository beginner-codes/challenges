# Challenge 546 - K-th Element of a Binary Sorted List

Given two positive integers `n` and `k`, generate all binaries between the integers `0` and `(2^n) - 1`, inclusive. These binaries will be sorted in descending order according to the number of 1's in them, if there is a tie, we choose the lowest numerical value. Return the k-th element from the sorted list created.

For `n = 3` and `k = 5` for example, the numbers from `0` to `7` (`7 = (2^3) - 1`), make the binary list:
```python
["0b0", "0b1", "0b10", "0b11", "0b100", "0b101", "0b110", "0b111"]
```
When sorted by the rules, we have:
```python
["0b111", "0b11", "0b101", "0b110", "0b1", "0b10", "0b100", "0b0"]
```
And `"0b1"` is the fifth element on it.

## Examples
```python
kth_binary_inlist(3, 5) ➞ "0b1"
# ["0b111", "0b11", "0b101", "0b110", "0b1", "0b10", "0b100", "0b0"]

kth_binary_inlist(4, 10) ➞ "0b1010"
# ["0b1111", "0b111", "0b1011", "0b1101", "0b1110", "0b11", "0b101", "0b110", "0b1001", "0b1010", "0b1100", "0b1", "0b10", "0b100", "0b1000", "0b0"]

kth_binary_inlist(5, 16) ➞ "0b11100"
# ["0b11111", "0b1111", "0b10111", "0b11011", "0b11101", "0b11110", "0b111", "0b1011", "0b1101", "0b1110", "0b10011", "0b10101", "0b10110", "0b11001", "0b11010", "0b11100", "0b11", "0b101", "0b110", "0b1001", "0b1010", "0b1100", "0b10001", "0b10010", "0b10100", "0b11000", "0b1", "0b10", "0b100", "0b1000", "0b10000", "0b0"]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def kth_binary_inlist(scale: list[int|str]) -> str:
    return "" # Put your code here!!!


test(546, kth_binary_inlist)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            3,
            5
        ],
        "return": "0b1"
    },
    {
        "args": [
            5,
            16
        ],
        "return": "0b11100"
    },
    {
        "args": [
            4,
            10
        ],
        "return": "0b1010"
    },
    {
        "args": [
            10,
            5
        ],
        "return": "0b1110111111"
    },
    {
        "args": [
            7,
            10
        ],
        "return": "0b101111"
    }
]
```
## Credits

Found on Edabit: [K-th Element of a Binary Sorted List](https://edabit.com/challenge/XDgNNWhxKemaurSGB)
