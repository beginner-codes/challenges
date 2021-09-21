# Challenge 338 - Digit Distance

The digit distance between two numbers is the total value of the difference between each pair of digits.

To illustrate:
```python
digit_distance(234, 489) ➞ 12
# Since |2 - 4| + |3 - 8| + |4 - 9| = 2 + 5 + 5
```
Create a function that returns the digit distance between two integers.

## Examples
```python
digit_distance(121, 599) ➞ 19

digit_distance(12, 12) ➞ 0

digit_distance(10, 20) ➞ 1
```
## Notes

- Both integers will be exactly the same length.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def digit_distance(num_a: int, num_b: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(digit_distance(121, 599), 19)

    def test_2(self):
        self.assertEqual(digit_distance(12, 12), 0)

    def test_3(self):
        self.assertEqual(digit_distance(10, 20), 1)

    def test_4(self):
        self.assertEqual(digit_distance(12345678, 23456789), 8)

    def test_5(self):
        self.assertEqual(digit_distance(5555, 6666), 4)

    def test_6(self):
        self.assertEqual(digit_distance(105, 777), 15)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Digit Distance](https://edabit.com/challenge/8xLnFm4HW4bzJrqjc)
