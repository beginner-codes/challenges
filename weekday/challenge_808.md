# Challenge 808 - Digital Decipher

In Digital Decipher, decoding is done by the simple subtraction of numbers in the key and the corresponding characters on a given list. You may want to solve this challenge before proceeding further.

Create a function that takes two arguments; a positive integer and a list of integers and returns a decoded message as string.

Assign a unique number to each letter of the alphabet.
```
 a  b  c  d  e  f  g  h  i  j  k  l  m
 1  2  3  4  5  6  7  8  9  10 11 12 13
 n  o  p  q  r  s  t  u  v  w  x  y  z
 14 15 16 17 18 19 20 21 22 23 24 25 26
```
There are some variations on the rules of encipherment. One version of the cipher rules are outlined below:
```
eMessage = [20, 12, 18, 30, 21]
key = 1939

digital_decipher(eMessage, key) ➞ "scout"
```
Subtract each key digit from eMessage consecutive digits:
```
  20 12 18 30 21
-  1  9  3  9  1
 ---------------
  19  3 15 21 20
```
Write the corresponding number against each character:
```
 s  c  o  u  t
19  3 15 21 20
```
See the below example for a better understanding:
```
eMessage = [14, 10, 22, 29, 6, 27, 19, 18, 6, 12, 8]
key = 1939

digital_decipher(eMessage, key) ➞ "masterpiece"

  14 10 22 29  6 27 19 18  6  12 8
-  1  9  3  9  1  9  3  9  1  9  3
  --------------------------------
  13  1 19 20  5 18 16  9  5  3  5
   m  a  s  t  e  r  p  i  e  c  e
```
Examples
```python
digital_decipher([20, 12, 18, 30, 21], 1939) ➞ "scout"

digital_decipher([15, 17, 14, 17, 19, 7, 21, 7, 2, 20, 20], 12) ➞ "nomoretears"
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


def digital_decipher(cipher: list[int], key: int) -> str:
    return ""  # Put your code here!!!


test(808, digital_decipher)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            [
                17,
                10,
                15,
                16,
                20,
                29,
                5,
                21
            ],
            1947
        ],
        "return": "pakistan"
    },
    {
        "args": [
            [
                14,
                10,
                22,
                29,
                6,
                27,
                19,
                18,
                6,
                12,
                8
            ],
            1939
        ],
        "return": "masterpiece"
    },
    {
        "args": [
            [
                15,
                17,
                14,
                17,
                19,
                7,
                21,
                7,
                2,
                20,
                20
            ],
            12
        ],
        "return": "nomoretears"
    },
    {
        "args": [
            [
                20,
                12,
                18,
                30,
                21
            ],
            1939
        ],
        "return": "scout"
    },
    {
        "args": [
            [
                17,
                10,
                17,
                14,
                20,
                29,
                7,
                19,
                2,
                18,
                24,
                11,
                16,
                27,
                9,
                10
            ],
            1965
        ],
        "return": "pakistanairforce"
    }
]
```

## Credits

Found on Edabit: [Digital Decipher](https://edabit.com/challenge/pyDemMDspSSFdWsh4)
