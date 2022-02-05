# Challenge 410 - Simple Numbers

A number that has N digits (enumerated d1, d2, ..., dN), is *simple* if the following condition is true:
```
X = d1^1 + d2^2 + ... + dN^N
```
**Examples of Simple Numbers:**
```
89 = 8^1 + 9^2

135 = 1^1 + 3^2 + 5^3
```
Create a function which returns a list of all the Simple Numbers that exist within a given range between `a` and `b` (inclusive).

## Examples
```python
simple_numbers(1, 10) ➞ [1, 2, 3, 4, 5, 6, 7, 8, 9]

simple_numbers(1, 100) ➞ [1, 2, 3, 4, 5, 6, 7, 8, 9, 89]

simple_numbers(90, 100) ➞ []
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def simple_numbers(start: int, end: int) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(simple_numbers(1, 10), [1, 2, 3, 4, 5, 6, 7, 8, 9])

    def test_2(self):
        self.assertEqual(simple_numbers(1, 100), [1, 2, 3, 4, 5, 6, 7, 8, 9, 89])

    def test_3(self):
        self.assertEqual(simple_numbers(10, 89), [89])

    def test_4(self):
        self.assertEqual(simple_numbers(10, 100), [89])

    def test_5(self):
        self.assertEqual(simple_numbers(90, 100), [])

    def test_6(self):
        self.assertEqual(simple_numbers(90, 150), [135])

    def test_7(self):
        self.assertEqual(simple_numbers(50, 150), [89, 135])

    def test_8(self):
        self.assertEqual(simple_numbers(10, 150), [89, 135])

    def test_9(self):
        self.assertEqual(simple_numbers(89, 135), [89, 135])

    def test_10(self):
        self.assertEqual(
            simple_numbers(100, 32253), [135, 175, 518, 598, 1306, 1676, 2427]
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Simple Numbers](https://edabit.com/challenge/FqFGnnffKRo8LKQKP)
