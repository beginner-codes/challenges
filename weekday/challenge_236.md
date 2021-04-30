# Challenge 236 - Sum of Odd and Even Numbers

Write a function that takes a list of numbers and returns a tuple with two elements:

- The first element should be the sum of all even numbers in the list.
- The second element should be the sum of all odd numbers in the list.

## Example
```python
sum_odd_and_even([1, 2, 3, 4, 5, 6]) ➞ (12, 9)
# 2 + 4 + 6 = 12 and 1 + 3 + 5 = 9

sum_odd_and_even([-1, -2, -3, -4, -5, -6]) ➞ (-12, -9))

sum_odd_and_even([0, 0]) ➞ (0, 0))
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def sum_odd_and_even(numbers: list[int]) -> tuple[int, int]:
    return 0, 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(sum_odd_and_even([1, 2, 3, 4, 5, 6]), (12, 9))

    def test_2(self):
        self.assertEqual(sum_odd_and_even([-1, -2, -3, -4, -5, -6]), (-12, -9))

    def test_3(self):
        self.assertEqual(sum_odd_and_even([0, 0]), (0, 0))

    def test_4(self):
        self.assertEqual(sum_odd_and_even([]), (0, 0))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sum of Odd and Even Numbers](https://edabit.com/challenge/5XXXppAdfcGaootD9)
