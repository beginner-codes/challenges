# Challenge 281 - Get the Excel Column

Excel column names are in the following format:
```
A, B, ..., Z, AA, ..., AZ, BA, ..., ZZ, AAA, AAB, ...
```
Write a function that returns the column number from the column name.

## Examples
```python
column("A") ➞ 1

column("Z") ➞ 26

column("AA") ➞ 27

column("BA") ➞ 53
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def column(column_label: str) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEquals(column("A"), 1)

    def test_2(self):
        self.assertEquals(column("B"), 2)

    def test_3(self):
        self.assertEquals(column("Z"), 26)

    def test_4(self):
        self.assertEquals(column("AA"), 27)

    def test_5(self):
        self.assertEquals(column("BA"), 53)

    def test_6(self):
        self.assertEquals(column("BB"), 54)

    def test_7(self):
        self.assertEquals(column("CW"), 101)

    def test_8(self):
        self.assertEquals(column("DD"), 108)

    def test_9(self):
        self.assertEquals(column("PQ"), 433)

    def test_10(self):
        self.assertEquals(column("ZZ"), 702)

    def test_11(self):
        self.assertEquals(column("ABC"), 731)

    def test_12(self):
        self.assertEquals(column("ZZT"), 18272)

    def test_13(self):
        self.assertEquals(column("STVW"), 348059)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Get the Excel Column](https://edabit.com/challenge/9S9k2h4ZnDeyzXEgW)
