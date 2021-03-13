# Challenge 202 - Concert Seats

Create a function that determines whether each seat can "see" the front-stage. A number can "see" the front-stage if it is strictly greater than the number before it.

Everyone can see the front-stage in this example:
```python
# FRONT STAGE
[[1, 2, 3, 2, 1, 1],
 [2, 4, 4, 3, 2, 2],
 [5, 5, 5, 5, 4, 4],
 [6, 6, 7, 6, 5, 5]]

# Starting from the left, the 6 > 5 > 2 > 1, so all numbers can see.
# 6 > 5 > 4 > 2 - so all numbers can see, etc.
```

Not everyone can see the front-stage in the example below:
```python
# FRONT STAGE
[[1, 2, 3,  2, 1, 1], 
 [2, 4, 4,  3, 2, 2], 
 [5, 5, 5, 10, 4, 4], 
 [6, 6, 7,  6, 5, 5]]

# The 10 is directly in front of the 6 and blocking its view.
```
The function should return `True` if every number can see the front-stage, and `False` if even a single number cannot.

## Examples
```python
can_see_stage([
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
]) ➞ True

can_see_stage([
  [0, 0, 0],
  [1, 1, 1],
  [2, 2, 2]
]) ➞ True

can_see_stage([
  [2, 0, 0], 
  [1, 1, 1], 
  [2, 2, 2]
]) ➞ False

can_see_stage([
  [1, 0, 0],
  [1, 1, 1],
  [2, 2, 2]
]) ➞ False
```
## Notes

- Numbers must be strictly greater than the number in front of it.
- All numbers within the lists will be whole numbers greater than or equal to zero.  

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def can_see_stage(rows: list[list[int]]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(can_see_stage([[1, 2, 3], [4, 5, 6], [7, 8, 9]]))

    def test_2(self):
        self.assertFalse(can_see_stage([[1, 2, 2], [1, 2, 3], [4, 4, 4]]))

    def test_3(self):
        self.assertFalse(can_see_stage([[1, 1, 2], [5, 2, 3], [4, 4, 4]]))

    def test_4(self):
        self.assertTrue(can_see_stage([[1, 1, 2], [5, 2, 3], [6, 4, 4]]))

    def test_5(self):
        self.assertTrue(can_see_stage([[0, 0, 0], [1, 1, 1], [2, 2, 2]]))

    def test_6(self):
        self.assertFalse(can_see_stage([[2, 0, 0], [1, 1, 1], [2, 2, 2]]))

    def test_7(self):
        self.assertFalse(can_see_stage([[1, 0, 0], [1, 1, 1], [2, 2, 2]]))

    def test_8(self):
        self.assertTrue(
            can_see_stage(
                [
                    [1, 2, 3, 2, 1, 1],
                    [2, 4, 4, 3, 2, 2],
                    [5, 5, 5, 5, 4, 4],
                    [6, 6, 7, 6, 5, 5],
                ]
            ),
            True,
        )

    def test_(self):
        self.assertEqual(
            can_see_stage(
                [
                    [1, 2, 3, 2, 1, 1],
                    [2, 4, 4, 3, 2, 2],
                    [5, 5, 5, 10, 4, 4],
                    [6, 6, 7, 6, 5, 5],
                ]
            ),
            False,
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Concert Seats](https://edabit.com/challenge/xbjDMxzpFcsAWKp97)
