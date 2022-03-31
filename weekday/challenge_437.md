# Challenge 437 - Count How Many Times an Element is Repeated

Given a list, create a function that returns a dictionary detailing how many times each element was repeated.

## Examples
```python
count_repetitions(["cat", "dog", "cat", "cow", "cow", "cow"]) ➞ { cow: 3, cat: 2, dog: 1 }

count_repetitions([1, 5, 5, 5, 12, 12, 0, 0, 0, 0, 0, 0]) ➞ { 0: 6, 5: 3, 12: 2, 1: 1 }

count_repetitions(["Infinity", "null", "Infinity", "null", "null"]) ➞ { "null": 3, "Infinity": 2}
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import TypeVar
import unittest


T = TypeVar("T")


def count_repetitions(items: list[T]) -> dict[T, int]:
    return {}  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            count_repetitions(["cat", "dog", "cat", "cow", "cow", "cow"]),
            {"cow": 3, "cat": 2, "dog": 1},
        )

    def test_2(self):
        self.assertEqual(
            count_repetitions([1, 5, 5, 5, 12, 12, 0, 0, 0, 0, 0, 0]),
            {0: 6, 5: 3, 12: 2, 1: 1},
        )

    def test_3(self):
        self.assertEqual(
            count_repetitions(["Infinity", "null", "Infinity", "null", "null"]),
            {"null": 3, "Infinity": 2},
        )

    def test_4(self):
        self.assertEqual(
            count_repetitions(["a", "b", "c", "a", "b", "a"]), {"a": 3, "b": 2, "c": 1}
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Count How Many Times an Element is Repeated](https://edabit.com/challenge/gDtHS9cAy8Fs2X7pH)
