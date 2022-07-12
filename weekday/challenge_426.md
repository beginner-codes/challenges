# Challenge 426 - Greater Than the Sum?

For each number in a list, check if that number is greater than the sum of all numbers that appear before it in the list. If all numbers in the list pass this test, return `True`. Return `False` otherwise.

## Examples
```python
greater_than_sum([2, 3, 7, 13, 28]) ➞ True

# 3 > 2 = True
# 7 > 2 + 3 = True
# 13 > 2 + 3 + 7 = True
# 28 > 2 + 3 + 7 + 13 = True

greater_than_sum([1, 2, 4, 6, 13]) ➞ False

# 2 > 1 = True
# 4 > 1 + 2 = True
# 6 > 1 + 2 + 4 = False
# 13 > 1 + 2 + 4 + 6 = False
```
## Notes

- The first number in any list will always pass the test.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def greater_than_sum(nums: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertFalse(greater_than_sum([1, -2, 11, 26]))

    def test_2(self):
        self.assertTrue(greater_than_sum([5, 8, 18, 32, 67, 131, 265, 529, 1056, 2115]))

    def test_3(self):
        self.assertTrue(greater_than_sum([8, 29, 62, 115, 232]))

    def test_4(self):
        self.assertFalse(
            greater_than_sum([5, 7, 15, 52, 88, 173, 346, 686, 1393, 2765])
        )

    def test_5(self):
        self.assertTrue(greater_than_sum([1, 25, 35, 74, 159, 305, 623]))

    def test_6(self):
        self.assertFalse(greater_than_sum([21, 40, 58, 134, 250]))

    def test_7(self):
        self.assertTrue(greater_than_sum([9, 32, 60, 107, 223, 442, 894, 1782, 3564]))

    def test_8(self):
        self.assertFalse(greater_than_sum([4, 26, 51, 103, 204, 412, 821, 1638, 3257]))

    def test_9(self):
        self.assertFalse(greater_than_sum([16, 35, 51, 120]))

    def test_10(self):
        self.assertFalse(greater_than_sum([-4, 1, 2, 14, 9, 44, 67, 131, 286]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Greater Than the Sum?](https://edabit.com/challenge/ZQhRtfh9CB8aSwvrc)
