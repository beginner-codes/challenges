# Challenge 312 - Counting Instances Created from a Class

Write a `Composer` class that has a class variable `count` which counts the total number of instances created.

## Examples
```python
# Just finished writing the Composer class
Composer.count ➞ 0

c1 = Composer("Ludvig van Beethoven", 1770, "Germany")
Composer.count ➞ 1

c2 = Composer("Wolfgang Amadeus Mozart", 1756, "Austria")
c3 = Composer("Johannes Brahms", 1833, "Germany")
Composer.count ➞ 3
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


class Composer:
    count: int  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(Composer.count, 0)

    def test_2(self):
        c1 = Composer("Ludvig van Beethoven", 1770, "Germany")
        self.assertEqual(Composer.count, 1)

    def test_3(self):
        c2 = Composer("Wolfgang Amadeus Mozart", 1756, "Austria")
        c3 = Composer("Johannes Brahms", 1833, "Germany")
        self.assertEqual(Composer.count, 3)

    def test_4(self):
        c4 = Composer("Richard Wagner", 1813, "Germany")
        c5 = Composer("Claude Debussy", 1862, "France")
        c6 = Composer("Richard Tchaikovsky", 1840, "Russia")
        c7 = Composer("Frederic Chopin", 1810, "Poland")
        self.assertEqual(Composer.count, 7)

    def test_5(self):
        c8 = Composer("Joseph Haydn", 1732, "Austria")
        self.assertEqual(Composer.count, 8)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Counting Instances Created from a Class](https://edabit.com/challenge/TkbgxTEn7rxd9hmx7)
