# Challenge 304 - Iterated Square Root

The iterated square root of a number is the number of times the square root function must be applied to bring the number strictly under 2.

Given an integer, return its iterated square root. Return `"invalid"` if it is negative.

## Examples
```python
i_sqrt(1) ➞ 0

i_sqrt(2) ➞ 1

i_sqrt(7) ➞ 2

i_sqrt(27) ➞ 3

i_sqrt(256) ➞ 4

i_sqrt(-1) ➞ "invalid"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from typing import Union
import unittest


def iterated_sqrt(n: int) -> Union[int, str]:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(iterated_sqrt(1), 0)

    def test_2(self):
        self.assertEqual(iterated_sqrt(2), 1)

    def test_3(self):
        self.assertEqual(iterated_sqrt(7), 2)

    def test_4(self):
        self.assertEqual(iterated_sqrt(27), 3)

    def test_5(self):
        self.assertEqual(iterated_sqrt(256), 4)

    def test_6(self):
        self.assertEqual(iterated_sqrt(-1), "invalid")

    def test_7(self):
        self.assertEqual(iterated_sqrt(25), 3)

    def test_8(self):
        self.assertEqual(iterated_sqrt(59), 3)

    def test_9(self):
        self.assertEqual(iterated_sqrt(113), 3)

    def test_37(self):
        self.assertEqual(iterated_sqrt(4294967296), 6)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Iterated Square Root](https://edabit.com/challenge/x5o7jTvzXjujvrh6t)
