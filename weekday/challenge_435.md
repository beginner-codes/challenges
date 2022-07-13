# Challenge 435 - The List Twins

Create a function that takes a list and returns the index at which the bisection would give you two sub lists with equal sums.

## Examples
```python
twins([10, 20, 30, 5, 40, 50, 40, 15]) ➞ 5
# foundIndex 5 : [10+20+30+5+40]=[50+40+15]

twins([1, 2, 3, 4, 5, 5]) ➞ 4
# [1, 2, 3, 4] [5, 5]

twins([3, 3]) ➞ 1
```
## Notes

- Return only the index of the bisection, not the bisected list.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def twins(numbers: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(twins([1, 2, 3, 4, 5, 5]), 4)

    def test_2(self):
        self.assertEqual(twins([3, 3]), 1)

    def test_3(self):
        self.assertEqual(twins([10, 20, 30, 5, 40, 50, 40, 15]), 5)

    def test_4(self):
        self.assertEqual(twins([3, 4, 6, 7, 6]), 3)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [The List Twins](https://edabit.com/challenge/9BJzrtpdMP8JFQg74)
