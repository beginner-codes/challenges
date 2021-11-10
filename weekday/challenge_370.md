# Challenge 370 - Filtering by Star Rating

Given a dictionary of some items with star ratings and a specified star rating, create a function that returns a new dictionary of items which match the specified star rating. Return `"No results found"` if no item matches the star rating given.

## Examples
```python
filter_by_rating({
  "Luxury Chocolates" : "*****",
  "Tasty Chocolates" : "****",
  "Aunty May Chocolates" : "*****",
  "Generic Chocolates" : "***"
}, "*****") ➞ {
  "Luxury Chocolates" : "*****",
  "Aunty May Chocolates" : "*****"
}

filter_by_rating({
  "Continental Hotel" : "****",
  "Big Street Hotel" : "**",
  "Corner Hotel" : "**",
  "Trashviews Hotel" : "*",
  "Hazbins" : "*****"
}, "*") ➞ {
  "Trashviews Hotel" : "*"
}

filter_by_rating({
  "Solo Restaurant" : "***",
  "Finest Dinings" : "*****",
  "Burger Stand" : "***"
}, "****") ➞ "No results found"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def filter_by_rating(brands: dict[str, str], rating: str) -> dict[str, str] | str:
    return "No results found"  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertDictEqual(
            filter_by_rating(
                {
                    "Brand A": "*",
                    "Brand B": "*****",
                    "Brand C": "*",
                    "Brand D": "**",
                    "Brand E": "****",
                    "Brand F": "*****",
                    "Brand G": "****",
                    "Brand H": "****",
                    "Brand I": "*****",
                    "Brand K": "***",
                    "Brand L": "*****",
                    "Brand M": "***",
                    "Brand N": "*",
                    "Brand O": "***",
                    "Brand P": "*****",
                    "Brand Q": "**",
                    "Brand R": "****",
                },
                "***",
            ),
            {"Brand K": "***", "Brand M": "***", "Brand O": "***"},
        )

    def test_2(self):
        self.assertDictEqual(
            filter_by_rating(
                {
                    "Brand A": "*",
                    "Brand B": "***",
                    "Brand C": "**",
                    "Brand D": "*****",
                    "Brand E": "*",
                    "Brand F": "****",
                    "Brand G": "*****",
                    "Brand H": "*****",
                    "Brand I": "**",
                    "Brand K": "*",
                    "Brand L": "*",
                    "Brand M": "***",
                    "Brand N": "*",
                    "Brand O": "*",
                    "Brand P": "**",
                    "Brand Q": "**",
                    "Brand R": "****",
                    "Brand S": "****",
                    "Brand T": "**",
                    "Brand U": "*",
                    "Brand V": "*",
                    "Brand W": "*",
                    "Brand X": "***",
                    "Brand Y": "*****",
                    "Brand Z": "****",
                },
                "**",
            ),
            {
                "Brand C": "**",
                "Brand I": "**",
                "Brand P": "**",
                "Brand Q": "**",
                "Brand T": "**",
            },
        )

    def test_7(self):
        self.assertDictEqual(
            filter_by_rating({"Brand A": "**", "Brand B": "*", "Brand C": "*"}, "**"),
            {"Brand A": "**"},
        )

    def test_8(self):
        self.assertDictEqual(
            filter_by_rating(
                {
                    "Brand A": "****",
                    "Brand B": "*",
                    "Brand C": "****",
                    "Brand D": "***",
                    "Brand E": "*****",
                },
                "**",
            ),
            "No results found",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Filtering by Star Rating](https://edabit.com/challenge/qM6zWQM7gdfPgE9Hh)
