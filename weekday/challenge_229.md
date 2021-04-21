# Challenge 229 - Sum Primes

Create a function that takes a list of numbers and returns the sum of all prime numbers in the list.

## Examples
```python
sum_primes([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]) ➞ 17

sum_primes([2, 3, 4, 11, 20, 50, 71]) ➞ 87

sum_primes([]) ➞ None
```
## Notes

- Given numbers won't exceed 101.
- A prime number is a number which has exactly two divisors.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def sum_primes(nums: list[int]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(sum_primes([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]), 17)

    def test_2(self):
        self.assertEqual(sum_primes([2, 3, 4, 11, 20, 50, 71]), 87)

    def test_3(self):
        self.assertEqual(sum_primes([19, 21, 24, 27, 30, 37]), 56)

    def test_4(self):
        self.assertEqual(sum_primes([69, 79, 87, 97, 101]), 277)

    def test_5(self):
        self.assertEqual(sum_primes([53, 59, 28, 50, 45, 33, 61]), 173)

    def test_6(self):
        self.assertEqual(sum_primes([]), None)

    def test_7(self):
        self.assertEqual(sum_primes([11, 11, 11, 11, 11, 22, 22, 22]), 55)

    def test_8(self):
        self.assertEqual(sum_primes([67, 24, 58, 28, 71, 73, 99]), 211)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Sum of Prime Numbers](https://edabit.com/challenge/GAbxxcsKoLGKtwjRB)
