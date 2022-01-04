# Challenge 385 - Adding Both Ends Together

Given a list of numbers, of any length, create a function which counts how many of those numbers pass the following criteria: the first and last digits of a number must add to 10.

## Examples
```python
ends_add_to_10([19, 46, 2098]) ➞ 3

ends_add_to_10([33, 44, -55]) ➞ 1

ends_add_to_10([]) ➞ 0
```
## Notes

- All items in the list will be numbers.
- Ignore negative signs.
- If given an empty list, return `0`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def ends_add_to_10(numbers: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(ends_add_to_10([19, 46, 2098]), 3)

    def test_2(self):
        self.assertEqual(ends_add_to_10([33, 44, -55]), 1)

    def test_3(self):
        self.assertEqual(ends_add_to_10([]), 0)

    def test_4(self):
        self.assertEqual(ends_add_to_10([-91, 55, -33]), 2)

    def test_5(self):
        self.assertEqual(
            ends_add_to_10([100, -10, 1, 3, 2, 5, 2]), 1
        )  # 5 should count.

    def test_6(self):
        self.assertEqual(ends_add_to_10([19, 28, 37, 46, 55, 64, 73, 82, 91]), 9)

    def test_7(self):
        self.assertEqual(
            ends_add_to_10([-19, -28, -37, -46, -55, -64, -73, -82, -91]), 9
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Adding Both Ends Together](https://edabit.com/challenge/en35WbjkDF9ej59FW)
