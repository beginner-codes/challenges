# Challenge 356 - Subset Validation

Write a function that returns 'True' if all subsets in a list belong to a given set.

## Examples
```python
validate_subsets([[1, 2], [2, 3], [1, 3]], [1, 2, 3]) ➞ True

validate_subsets([[1, 2, 3], [2], [3], []], [1, 2, 3]) ➞ True

validate_subsets([[1, 2], [2, 3], [1, 4]], [1, 2, 3]) ➞ False

validate_subsets([[1, 2, 3, 4]], [1, 2, 3]) ➞ False
```
## Notes

- The empty set and the set itself are both valid subsets of a set (we are not talking about proper subsets here).
- The set and the subset will each have unique elements.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import TypeVar
import unittest


T = TypeVar("T")


def validate_subsets(subsets: list[list[T]], superset: list[T]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(validate_subsets([[1, 2], [2, 3], [1, 3]], [1, 2, 3]))

    def test_2(self):
        self.assertTrue(validate_subsets([[1, 2, 3], [2], [3], []], [1, 2, 3]))

    def test_3(self):
        self.assertFalse(validate_subsets([[1, 2], [2, 3], [1, 4]], [1, 2, 3]))

    def test_4(self):
        self.assertFalse(validate_subsets([[1, 2, 3, 4]], [1, 2, 3]))

    def test_5(self):
        self.assertTrue(validate_subsets([["a", "b"], ["b", "c"], ["a", "c"]], ["a", "b", "c"]))

    def test_6(self):
        self.assertTrue(validate_subsets([["a", "b", "c"], ["b"], ["c"], []], ["a", "b", "c"]))

    def test_7(self):
        self.assertFalse(validate_subsets([["a", "b"], ["b", "c"], ["a", "d"]], ["a", "b", "c"]))

    def test_8(self):
        self.assertFalse(validate_subsets([["a", "b", "c", "d"]], ["a", "b", "c"]))

    def test_9(self):
        self.assertTrue(validate_subsets([[True, False], [True]], [True, False]))

    def test_10(self):
        self.assertTrue(validate_subsets([[True], [False], []], [True, False]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Subset Validation](https://edabit.com/challenge/nrjJcg6XMcoCvKH8y)
