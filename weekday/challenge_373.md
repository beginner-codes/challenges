# Challenge 373 - All Numbers in List Are Prime

Create a function that takes a list and returns `True` if every number is prime. Otherwise, return `False`.

## Examples
```python
all_prime([7, 5, 2, 4, 6]) ➞ False

all_prime([2, 3, 5, 7, 13, 17, 19, 23, 29]) ➞ True

all_prime([1, 5, 3]) ➞ False
```
## Notes

- `1` is not a prime number.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def all_prime(numbers: list[int]) -> bool:
    return False  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertFalse(all_prime([7, 5, 2, 4, 6]))

    def test_2(self):
        self.assertTrue(all_prime([2, 3, 5, 7, 13, 17, 19, 23, 29]))

    def test_3(self):
        self.assertFalse(all_prime([1, 5, 3]))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [All Numbers in List Are Prime](https://edabit.com/challenge/6M4gYkxWTsE6Rxhge)
