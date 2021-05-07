# Challenge 241 - Count Palindrome Numbers in a Range

Create a function that returns the number of palindrome numbers in a specified range (inclusive).

For example, between 8 and 34, there are 5 palindromes: 8, 9, 11, 22 and 33. Between 1550 and 1552 there is exactly one palindrome: 1551.

## Examples
```python
count_palindromes(1, 10) ➞ 9

count_palindromes(555, 556) ➞ 1

count_palindromes(878, 898) ➞ 3
```
## Notes

- Single-digit numbers are trivially palindrome numbers.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def count_palindromes(start: int, end: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(count_palindromes(1, 10), 9)

    def test_2(self):
        self.assertEqual(count_palindromes(555, 556), 1)

    def test_3(self):
        self.assertEqual(count_palindromes(878, 898), 3)

    def test_4(self):
        self.assertEqual(count_palindromes(8, 34), 5)

    def test_5(self):
        self.assertEqual(count_palindromes(1550, 1556), 1)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Count Palindrome Numbers in a Range](https://edabit.com/challenge/QEDPxbfHjvWXQQtpH)
