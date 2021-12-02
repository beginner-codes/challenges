# Challenge 381 - Joining Digits Together

Create a function which takes a number as input and returns all numbers up to and including that number, joined together in a string. Separate each digit from each other with the character `"-"`.

## Examples
```python
join_digits(4) ➞ "1-2-3-4"

join_digits(11) ➞ "1-2-3-4-5-6-7-8-9-1-0-1-1"

join_digits(15) ➞ "1-2-3-4-5-6-7-8-9-1-0-1-1-1-2-1-3-1-4-1-5"
```
## Notes

- Remember to start at 1 and include the number as the last number.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def join_digits(n: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(join_digits(1), "1")

    def test_2(self):
        self.assertEqual(join_digits(2), "1-2")

    def test_3(self):
        self.assertEqual(join_digits(3), "1-2-3")

    def test_4(self):
        self.assertEqual(join_digits(4), "1-2-3-4")

    def test_5(self):
        self.assertEqual(join_digits(5), "1-2-3-4-5")

    def test_6(self):
        self.assertEqual(join_digits(6), "1-2-3-4-5-6")

    def test_7(self):
        self.assertEqual(join_digits(7), "1-2-3-4-5-6-7")

    def test_8(self):
        self.assertEqual(join_digits(8), "1-2-3-4-5-6-7-8")

    def test_9(self):
        self.assertEqual(join_digits(9), "1-2-3-4-5-6-7-8-9")

    def test_10(self):
        self.assertEqual(join_digits(10), "1-2-3-4-5-6-7-8-9-1-0")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Joining Digits Together](https://edabit.com/challenge/K6oxe3bvPqaQWxkFw)
