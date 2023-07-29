# Challenge 716 - The ECG Sequence

In the ECG Sequence (that always starts with the numbers 1 and 2), every number that succeeds is the smallest not already present in the sequence and that shares a factor (excluding 1) with its preceding number. Every number in the ECG Sequence (besides 1 and 2) has a different index from its natural index in a normal numeric sequence. See the example below to establish the ECG Sequence Index of number 3.
```python
# Find the smallest number that is not in sequence...
# This number shares a factor with the preceding?

SEQUENCE = [1, 2]

3 = no factors shared with 2
4 = shares factor 2 with number 2

SEQUENCE = [1, 2, 4]

3 = no factors shared with 4
5 = no factors shared with 4
6 = shares factor 2 with number 4

SEQUENCE = [1, 2, 4, 6]

3 = shares factor 3 with number 6

SEQUENCE = [1, 2, 4, 6, 3]
```
Number 3 is at index 4 in the ECG Sequence.

Given an integer `n` implement a function that returns its ECG Sequence Index.

## Examples
```python
ecg_sequence_index(3) ➞ 4

ecg_sequence_index(5) ➞ 9

ecg_sequence_index(7) ➞ 13
```
## Notes

- ECG is the acronym for the electrocardiogram: if you try to graphically represent the trend of the sequence, a similar scheme appears.
- Curiosity: every odd prime `p` in the sequence is preceded by `2p` and followed by `3p`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def ecg_sequence_index(number: int) -> int:
    return 0  # Put your code here!!!


test(716, ecg_sequence_index)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            75
        ],
        "return": 68
    },
    {
        "args": [
            101
        ],
        "return": 188
    },
    {
        "args": [
            5
        ],
        "return": 9
    },
    {
        "args": [
            7
        ],
        "return": 13
    },
    {
        "args": [
            3
        ],
        "return": 4
    }
]
```
## Credits

Found on Edabit: [The ECG Sequence](https://edabit.com/challenge/9Px2rkc9TPhK54wDb)
