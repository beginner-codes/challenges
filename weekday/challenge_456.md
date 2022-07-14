# Challenge 456 - A Simple Check

Create a function which takes two positive integers. These numbers are simultaneously decreased by `1` until the smaller one reaches `0`.

During this process, the greater number can be divisible by the smaller one. Your task is to count how many times that happens.

_Example 1_
```python
a = 3, b = 5  # 5 is not divisible by 3
a = 2, b = 4  # decreased by 1, 4 is divisible by 2
a = 1, b = 3  # decreased by 1, 3 is divisible by 1
a = 0, b = 2  # decreased by 1, the smaller number is 0, End
```
The result should be `2`

_Example 2_
```python
a = 8, b = 4  # 8 is divisible by 4
a = 7, b = 3  # decreased by 1, 7 is not divisible by 3
a = 6, b = 2  # decreased by 1, 6 is divisible by 2
a = 5, b = 1  # decreased by 1, 5 is divisible by 1
a = 4, b = 0  # decreased by 1, the smaller number is 0, End
```
The result should be `3`

## Examples
```python
simple_check(3, 5) ➞ 2

simple_check(8, 4) ➞ 3

simple_check(54, 17) ➞ 1
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 
```json
[
    {
        "args": [
            3,
            5
        ],
        "return": 2
    },
    {
        "args": [
            10,
            1
        ],
        "return": 1
    },
    {
        "args": [
            7,
            7
        ],
        "return": 7
    },
    {
        "args": [
            16,
            32
        ],
        "return": 5
    },
    {
        "args": [
            42,
            21
        ],
        "return": 4
    },
    {
        "args": [
            54,
            17
        ],
        "return": 1
    },
    {
        "args": [
            150080,
            150032
        ],
        "return": 10
    }
]
```
## Credits

Found on Edabit: [A Simple Check](https://edabit.com/challenge/hQRuQguN4bKyM2gik)
