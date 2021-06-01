# Challenge 258 - Tuck In List

Create a function that takes two lists and insert the second list in the middle of the first list.

## Examples
```python
tuck_in([1, 10], [2, 3, 4, 5, 6, 7, 8, 9]) ➞ [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

tuck_in([15, 150], [45, 75, 35]) ➞ [15, 45, 75, 35, 150]

tuck_in([[1, 2], [5, 6]], [[3, 4]]) ➞ [[1, 2], [3, 4], [5, 6]]
```

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
from typing import Any
import unittest


def tuck_in(outer_list: list[Any], inner_list: list[Any]) -> list[Any]:
    return []  # Put your code here!!!`


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            tuck_in([1, 10], [2, 3, 4, 5, 6, 7, 8, 9]), [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
        )

    def test_2(self):
        self.assertListEqual(tuck_in([15, 150], [45, 75, 35]), [15, 45, 75, 35, 150])

    def test_3(self):
        self.assertListEqual(
            tuck_in(["bottom", "topping"], ["tomatosauce", "vegetables", "cheese"]),
            ["bottom", "tomatosauce", "vegetables", "cheese", "topping"],
        )

    def test_4(self):
        self.assertListEqual(
            tuck_in([[1, 2], [5, 6]], [[3, 4]]), [[1, 2], [3, 4], [5, 6]]
        )

    def test_5(self):
        self.assertListEqual(
            tuck_in([True, False], [False, True, None, None]),
            [True, False, True, None, None, False],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Tuck in Array](https://edabit.com/challenge/7ysTEDruHz2prcJQ9)
