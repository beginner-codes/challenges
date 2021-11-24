# Challenge 377 - Evaluating Factorials

Create a function that takes a list of factorial expressions and returns their sum.

## Examples
```python
eval_factorial(["2!", "3!"]) ➞ 8

eval_factorial(["5!", "4!", "2!"]) ➞ 146

eval_factorial(["0!", "1!"]) ➞ 2
```
## Notes

- `0!` and `1!` both equal 1.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def eval_factorial(number: list[str]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(eval_factorial(["2!", "3!"]), 8)

    def test_2(self):
        self.assertEqual(eval_factorial(["5!", "4!", "2!"]), 146)

    def test_3(self):
        self.assertEqual(eval_factorial(["0!", "1!"]), 2)

    def test_4(self):
        self.assertEqual(eval_factorial(["5!", "5!", "10!"]), 3629040)

    def test_5(self):
        self.assertEqual(eval_factorial(["6!", "3!"]), 726)

    def test_6(self):
        self.assertEqual(eval_factorial(["2!", "2!", "1!", "1!"]), 6)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Evaluating Factorials](https://edabit.com/challenge/ZwsHZLRqx3TLFk3CR)
