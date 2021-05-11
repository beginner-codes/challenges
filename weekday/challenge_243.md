# Challenge 243 - Get the Area of a Country

Create a function that takes a country's name and its area as arguments and returns the area of the country's proportion of the total world's landmass.

## Examples
```python
area_of_country("Russia", 17098242) ➞ "Russia is 11.48% of the total world's landmass"

area_of_country("USA", 9372610) ➞  "USA is 6.29% of the total world's landmass"

area_of_country("Iran", 1648195) ➞ "Iran is 1.11% of the total world's landmass"
```
## Notes

- The total world's landmass is 148,940,000km^2
- Round the result to two decimal places.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def area_of_country(country: str, land_area: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            area_of_country("USA", 9372610),
            "USA is 6.29% of the total world's landmass",
        )

    def test_2(self):
        self.assertEqual(
            area_of_country("Russia", 17098242),
            "Russia is 11.48% of the total world's landmass",
        )

    def test_3(self):
        self.assertEqual(
            area_of_country("Iran", 1648195),
            "Iran is 1.11% of the total world's landmass",
        )

    def test_4(self):
        self.assertEqual(
            area_of_country("India", 3287590),
            "India is 2.21% of the total world's landmass",
        )

    def test_5(self):
        self.assertEqual(
            area_of_country("China", 9706961),
            "China is 6.52% of the total world's landmass",
        )

    def test_6(self):
        self.assertEqual(
            area_of_country("Yemen", 527968),
            "Yemen is 0.35% of the total world's landmass",
        )

    def test_7(self):
        self.assertEqual(
            area_of_country("Switzerland", 41284),
            "Switzerland is 0.03% of the total world's landmass",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [The Primiera](https://edabit.com/challenge/bPzBa5JKvb6XFyKMs)
