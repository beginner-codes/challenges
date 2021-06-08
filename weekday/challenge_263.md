# Challenge 263 - Find the Discount

Create a function that takes two arguments: the original price and the discount percentage as integers and returns the final price after the discount.

## Examples
```python
calculate_discount(1500, 50) ➞ 750

calculate_discount(89, 20) ➞ 71.2

calculate_discount(100, 75) ➞ 25
```
## Notes

- Your answer should be rounded to two decimal places.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def calculate_discount(price: int, discount_percent: int) -> float:
    return 0.0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(calculate_discount(100, 75), 25)

    def test_2(self):
        self.assertEqual(calculate_discount(211, 50), 105.5)

    def test_3(self):
        self.assertEqual(calculate_discount(593, 61), 231.27)

    def test_4(self):
        self.assertEqual(calculate_discount(1693, 80), 338.6)

    def test_5(self):
        self.assertEqual(calculate_discount(700, 10), 630)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Find the Discount](https://edabit.com/challenge/cXnkmRdxqJrwdsP4n)
