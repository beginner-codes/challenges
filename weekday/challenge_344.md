# Challenge 344 - Percentage Changed

Create a function that takes an old price, a new price, and returns what percent the price decreased or increased. Round the percentage to the nearest whole percent.

## Examples
```python
percentage_changed("$800", "$600") ➞ "25% decrease"

percentage_changed("$1000", "$840") ➞ "16% decrease"

percentage_changed("$100", "$950") ➞ "850% increase"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def percentage_changed(old_price: str, new_price: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(percentage_changed("$800", "$600"), "25% decrease")

    def test_2(self):
        self.assertEqual(percentage_changed("$1000", "$840"), "16% decrease")

    def test_3(self):
        self.assertEqual(percentage_changed("$700", "$650"), "7% decrease")

    def test_4(self):
        self.assertEqual(percentage_changed("$100", "$950"), "850% increase")

    def test_5(self):
        self.assertEqual(percentage_changed("$450", "$460"), "2% increase")

    def test_6(self):
        self.assertEqual(percentage_changed("$1000", "$1500"), "50% increase")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Percentage Changed](https://edabit.com/challenge/7ZFrHepr336TBMsF5)
