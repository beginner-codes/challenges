# Challenge 341 - Is the Sum of Letters Even or Odd?

Create a function that takes a string and returns `True` if the sum of the position of every letter in the alphabet is even and `False` if the sum is odd.

## Examples
```python
is_letter_sum_even("i'am king")  ➞ True
# 9 + 1 + 13 + 11 + 9 + 14 + 7 = 64 (even)

is_letter_sum_even("True") ➞ True
# 20 + 18 + 21 + 5= 64 (even)

is_letter_sum_even("alexa") ➞ False
# 1 + 12 + 5 + 24 + 1= 43 (odd)
```
## Notes

- Case-insensitive.
- Ignore non-letter symbols.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def is_letter_sum_even(string: str) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertTrue(is_letter_sum_even("i'am king"))

    def test_2(self):
        self.assertTrue(is_letter_sum_even("True"))

    def test_3(self):
        self.assertFalse(is_letter_sum_even("alexa"))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Is the Sum of Letters Even or Odd?](https://edabit.com/challenge/Mm8SK7DCvzissCF2s)
