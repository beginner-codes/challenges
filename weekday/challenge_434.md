# Challenge 434 - Prime Factorization of an Integer

Create a function that returns a list containing the prime factors of whatever integer is passed to it.

## Examples
```python
prime_factors(20) ➞ [2, 2, 5]

prime_factors(100) ➞ [2, 2, 5, 5]

prime_factors(8912234) ➞ [2, 47, 94811]
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def prime_factors(number: int) -> list[int]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(prime_factors(20), [2, 2, 5])

    def test_2(self):
        self.assertEqual(prime_factors(100), [2, 2, 5, 5])

    def test_3(self):
        self.assertEqual(prime_factors(8912234), [2, 47, 94811])


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Prime Factorization of an Integer](https://edabit.com/challenge/8vBvgJMc2uQJpD6d7)
