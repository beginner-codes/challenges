# Challenge 405 - Anti Lists

Given two lists, return whether the two lists are opposites of each other. That means both lists are comprised only from elements `a` and `b` and the occurrences of these elements are swapped between the two lists.

## Examples
```python
is_anti_list(["1", "0", "0", "1"], ["0", "1", "1", "0"]) ➞ True

is_anti_list(["apples", "bananas", "bananas"], ["bananas", "apples", "apples"]) ➞ True

is_anti_list([3.14, True, 3.14], [3.14, False, 3.14]) ➞ False
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Any
import unittest


def is_anti_list(list_a: list[Any], list_b: list[Any]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_anti_list(["1", "0", "0", "1"], ["0", "1", "1", "0"]))

    def test_2(self):
        self.assertTrue(
            is_anti_list(
                ["apples", "bananas", "bananas"], ["bananas", "apples", "apples"]
            )
        )

    def test_3(self):
        self.assertFalse(is_anti_list([3.14, True, 3.14], [3.14, False, 3.14]))

    def test_4(self):
        self.assertFalse(is_anti_list([6.28, True, 6.28], [True, False, True]))

    def test_5(self):
        self.assertTrue(is_anti_list([int, str], [str, int]))

    def test_6(self):
        self.assertFalse(is_anti_list([3.14, True, 3.14], [3.14, True, 3.14]))

    def test_7(self):
        self.assertFalse(is_anti_list(["a", "b", "b", "a"], ["b", "b", "a", "a"]))

    def test_8(self):
        self.assertFalse(is_anti_list(["1", "2", "2", "2"], ["2", "2", "2", "1"]))

    def test_9(self):
        self.assertTrue(
            is_anti_list(
                [121, float, float, float, 121, float],
                [float, 121, 121, 121, float, 121],
            )
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Anti Lists](https://edabit.com/challenge/TDrfRh63jMCmqzGjv)
