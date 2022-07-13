# Challenge 351 - Fruit Juices

A fruit juice company tags their fruit juices by concatenating the first three letters of the words in a flavor's name, with its capacity.

Create a function that creates product IDs for different fruit juices.

## Examples
```python
get_drink_id("apple", "500ml") ➞ "APP500"

get_drink_id("pineapple", "45ml") ➞ "PIN45"

get_drink_id("passion fruit", "750ml") ➞ "PASFRU750"
```
## Notes

-  Capacity will be given as a string, and will always be given in ml.
- Return the letters in UPPERCASE.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def get_drink_id(string: str, capacity: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(get_drink_id("apple", "500ml"), "APP500")

    def test_2(self):
        self.assertEqual(get_drink_id("pineapple", "45ml"), "PIN45")

    def test_3(self):
        self.assertEqual(get_drink_id("orange", "750ml"), "ORA750")

    def test_4(self):
        self.assertEqual(get_drink_id("passion fruit", "1ml"), "PASFRU1")

    def test_5(self):
        self.assertEqual(get_drink_id("mango", "1000ml"), "MAN1000")

    def test_6(self):
        self.assertEqual(get_drink_id("very berry", "253ml"), "VERBER253")

    def test_7(self):
        self.assertEqual(get_drink_id("raspberry and lime", "350ml"), "RASANDLIM350")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Fruit Juices](https://edabit.com/challenge/Mv5qSgZKTLrLt9zzW)
