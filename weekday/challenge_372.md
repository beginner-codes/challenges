# Challenge 372 - Birthday Cake

Create a function which constructs a rectangular birthday cake, based on someone's name and age! Build it out of strings in a list and makes sure to surround the birthday message with the character that fits the rule:

- If the age is an even number, surround the message with `"#"`.
- If  the age is an odd number, surround the message with `"*"`.

Other important rules:

- The message should be in the format: `{age} Happy Birthday {name}! {age}`
- Leave a space between the edge of the cake and the age numbers.

## Examples
```python
get_birthday_cake("Jack", 10) ➞ [
  "##############################",
  "# 10 Happy Birthday Jack! 10 #",
  "##############################"
]

get_birthday_cake("Russell", 19) ➞ [
  "*********************************",
  "* 19 Happy Birthday Russell! 19 *",
  "*********************************"
]

get_birthday_cake("Isabelle", 2) ➞ [
  "################################",
  "# 2 Happy Birthday Isabelle! 2 #",
  "################################"
]
```
## Notes

- The amount of characters in the banner should be the same length as the message to pass the tests.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def get_birthday_cake(name: str, age: int) -> list[str]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertListEqual(
            get_birthday_cake("Jack", 10),
            [
                "##############################",
                "# 10 Happy Birthday Jack! 10 #",
                "##############################",
            ],
        )

    def test_2(self):
        self.assertListEqual(
            get_birthday_cake("Russell", 19),
            [
                "*********************************",
                "* 19 Happy Birthday Russell! 19 *",
                "*********************************",
            ],
        )

    def test_3(self):
        self.assertListEqual(
            get_birthday_cake("Isabelle", 2),
            [
                "################################",
                "# 2 Happy Birthday Isabelle! 2 #",
                "################################",
            ],
        )

    def test_4(self):
        self.assertListEqual(
            get_birthday_cake("Princess", 40),
            [
                "##################################",
                "# 40 Happy Birthday Princess! 40 #",
                "##################################",
            ],
        )

    def test_5(self):
        self.assertListEqual(
            get_birthday_cake("Maxwell", 85),
            [
                "*********************************",
                "* 85 Happy Birthday Maxwell! 85 *",
                "*********************************",
            ],
        )

    def test_6(self):
        self.assertListEqual(
            get_birthday_cake("Zenobia", 63),
            [
                "*********************************",
                "* 63 Happy Birthday Zenobia! 63 *",
                "*********************************",
            ],
        )

    def test_7(self):
        self.assertListEqual(
            get_birthday_cake("Adrian", 91),
            [
                "********************************",
                "* 91 Happy Birthday Adrian! 91 *",
                "********************************",
            ],
        )

    def test_8(self):
        self.assertListEqual(
            get_birthday_cake("Gayle", 28),
            [
                "###############################",
                "# 28 Happy Birthday Gayle! 28 #",
                "###############################",
            ],
        )

    def test_9(self):
        self.assertListEqual(
            get_birthday_cake("Jo", 69),
            [
                "****************************",
                "* 69 Happy Birthday Jo! 69 *",
                "****************************",
            ],
        )

    def test_10(self):
        self.assertListEqual(
            get_birthday_cake("Val", 80),
            [
                "#############################",
                "# 80 Happy Birthday Val! 80 #",
                "#############################",
            ],
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Birthday Cake](https://edabit.com/challenge/994QjWPmdhaR94DeF)
