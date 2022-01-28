# Challenge 404 - Emptying the Values

Given a list of values, return a list with each value replaced with the empty value of the same type.

More explicitly:

- Replace integers (e.g. `1`, `3`), whose type is int, with `0`
- Replace floats (e.g. `3.14`, `2.17`), whose type is float, with `0.0`
- Replace strings (e.g. `"abcde"`, `"x"`), whose type is str, with `"""`
- Replace booleans (`True`, `False`), whose type is bool, with `False`
- Replace lists (e.g. `[1, "a", 5]`, `[[4]]`), whose type is list, with `[]`
- Replace tuples (e.g. `(1,9,0)`, `(2,)`), whose type is tuple, with `tuple()`
- Replace sets (e.g. `{0,"a"}`, `{"b"}`), whose type is set, with `set()`

_Caution: Python interprets {} as the empty dictionary, not the empty set._
_`None`, whose type is `NoneType`, is preserved as `None`_

## Examples
```python
empty_values([1, 2, 3]) ➞ [0, 0, 0]

empty_values([7, 3.14, "cat"]) ➞ [0, 0.0, ""]

empty_values([[1, 2, 3], (1,2,3), {1,2,3}]) ➞ [[], (), set()]

empty_values([[7, 3.14, "cat"]]) ➞ [[]]

empty_values([None]) ➞ [None]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import TypeVar
import unittest


Value = TypeVar("Value")


def empty_values(values: list[Value]) -> list[Value]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(empty_values([1, 2, 3]), [0, 0, 0])

    def test_2(self):
        self.assertEqual(empty_values([7, 3.14, "cat"]), [0, 0.0, ""])

    def test_3(self):
        self.assertEqual(
            empty_values([[1, 2, 3], (1, 2, 3), {1, 2, 3}]), [[], (), set()]
        )

    def test_4(self):
        self.assertEqual(empty_values([[7, 3.14, "cat"]]), [[]])

    def test_5(self):
        self.assertEqual(empty_values([None]), [None])

    def test_6(self):
        self.assertEqual(
            empty_values([None, [None], (None, [None]), {None}, True, 7.0, 7, "None"]),
            [None, [], (), set(), False, 0.0, 0, ""],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Emptying the Values](https://edabit.com/challenge/zNNtsPBCE5FFXW7wn)
