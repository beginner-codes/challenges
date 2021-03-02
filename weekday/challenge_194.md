# Challenge 194 - Expensive Orders

Write a function that has two parameters: `orders` and `cost`. Return any orders that are greater than the cost.

## Examples
```python
expensive_orders({ "a": 3000, "b": 200, "c": 1050 }, 1000)
➞ { "a": 3000, "c": 1050 }

expensive_orders({ "Gucci Fur": 24600, "Teak Dining Table": 3200, "Louis Vutton Bag": 5550, "Dolce Gabana Heels": 4000 }, 20000)
➞ { "Gucci Fur": 24600 }

expensive_orders({ "Deluxe Burger": 35, "Icecream Shake": 4, "Fries": 5 }, 40)
➞ {}
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def expensive_orders(orders: dict[str, int], cost: int) -> dict[str, int]:
    return {}  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            expensive_orders({"a": 3000, "b": 200, "c": 1050}, 1000),
            {"a": 3000, "c": 1050},
        )

    def test_2(self):
        self.assertEqual(
            expensive_orders(
                {
                    "Gucci Fur": 24600,
                    "Teak Dining Table": 3200,
                    "Louis Vutton Bag": 5550,
                    "Dolce Gabana Heels": 4000,
                },
                20000,
            ),
            {"Gucci Fur": 24600},
        )

    def test_3(self):
        self.assertEqual(
            expensive_orders(
                {"Deluxe Burger": 35, "Icecream Shake": 4, "Fries": 5}, 40
            ),
            {},
        )

    def test_4(self):
        self.assertEqual(
            expensive_orders(
                {"Kyoto Ticket": 10, "Museum Exhibit": 30, "Kimono": 3000}, 5
            ),
            {"Kyoto Ticket": 10, "Museum Exhibit": 30, "Kimono": 3000},
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on /r/dailyprogrammer: [\[2018-04-23\] Challenge #358 \[Easy\] Decipher The Seven Segments](https://www.reddit.com/r/dailyprogrammer/comments/8eger3/20180423_challenge_358_easy_decipher_the_seven/)
