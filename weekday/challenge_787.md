# Challenge 787 - Digital Cipher

In a digital cipher, encoding is done by the simple addition of numbers in the key and the corresponding characters from a string.

Create a function that takes two arguments: a positive integer and a string, and returns an encoded list of integers.

Assign a unique number to each letter of the alphabet.
```
 a  b  c  d  e  f  g  h  i  j  k  l  m
 1  2  3  4  5  6  7  8  9  10 11 12 13

 n  o  p  q  r  s  t  u  v  w  x  y  z
 14 15 16 17 18 19 20 21 22 23 24 25 26
```
There are some variations on the rules for encoding a digital cipher. One version of the cipher rules are outlined below:
```python
message = "scout"
key = 1939

digital_cipher(message, key) ➞ [20, 12, 18, 30, 21]
```
Write the corresponding number against each character:
```
 s  c  o  u  t
19  3 15 21 20
```
Add to each obtained digit consecutive digits from the key:
```
   s  c  o  u  t
  19  3 15 21 20
 + 1  9  3  9  1
 ---------------
  20 12 18 30 21
```
See the below example for a better understanding:
```python
message = "masterpiece"
key = 1939

digital_cipher(message, key) ➞ [14, 10, 22, 29, 6, 27, 19, 18, 6, 12, 8]
```
```
   m  a  s  t  e  r  p  i  e  c  e
  13  1 19 20  5 18 16  9  5  3  5
+  1  9  3  9  1  9  3  9  1  9  3
  --------------------------------
  14 10 22 29  6 27 19 18  6  12 8
```
## Examples
```python
digital_cipher("scout", 1939) ➞ [20, 12, 18, 30, 21]

digital_cipher("masterpiece", 1939) ➞ [14, 10, 22, 29, 6, 27, 19, 18, 6, 12, 8]
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


def digital_cipher(string: str, key: int) -> list[int]:
    return []  # Put your code here!!!


test(787, digital_cipher)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "scout",
            1939
        ],
        "return": [
            20,
            12,
            18,
            30,
            21
        ]
    },
    {
        "args": [
            "masterpiece",
            1939
        ],
        "return": [
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
        ]
    },
    {
        "args": [
            "nomoretears",
            12
        ],
        "return": [
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
        ]
    }
]
```

## Credits

Found on Edabit: [Digital Cipher](https://edabit.com/challenge/WFmZesxp2GXQcT8PE)
