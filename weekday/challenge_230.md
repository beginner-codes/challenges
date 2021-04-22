# Challenge 230 - Loves Me, Loves Me Not...

*"Loves me, loves me not"* is a traditional game in which a person plucks off all the petals of a flower one by one, saying the phrase "Loves me" and "Loves me not" when determining whether the one that they love, loves them back.

Given a number of petals, return a string which repeats the phrases "Loves me" and "Loves me not" for every alternating petal, and return the last phrase in all caps. Remember to put a comma and space between phrases.

## Examples
```python
loves_me(3) ➞ "Loves me, Loves me not, LOVES ME"

loves_me(6) ➞ "Loves me, Loves me not, Loves me, Loves me not, Loves me, LOVES ME NOT"

loves_me(1) ➞ "LOVES ME"
```
## Notes

- Remember to return a string.
- The first phrase is always "Loves me".

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def loves_me(num_petals: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(loves_me(1), "LOVES ME")

    def test_2(self):
        self.assertEqual(loves_me(2), "Loves me, LOVES ME NOT")

    def test_3(self):
        self.assertEqual(loves_me(3), "Loves me, Loves me not, LOVES ME")

    def test_4(self):
        self.assertEqual(loves_me(4), "Loves me, Loves me not, Loves me, LOVES ME NOT")

    def test_5(self):
        self.assertEqual(
            loves_me(5), "Loves me, Loves me not, Loves me, Loves me not, LOVES ME"
        )

    def test_6(self):
        self.assertEqual(
            loves_me(6),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, LOVES ME NOT",
        )

    def test_7(self):
        self.assertEqual(
            loves_me(7),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, LOVES ME",
        )

    def test_8(self):
        self.assertEqual(
            loves_me(8),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, LOVES ME NOT",
        )

    def test_9(self):
        self.assertEqual(
            loves_me(9),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, LOVES ME",
        )

    def test_10(self):
        self.assertEqual(
            loves_me(10),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, "
            "LOVES ME NOT",
        )

    def test_11(self):
        self.assertEqual(
            loves_me(11),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, "
            "Loves me not, LOVES ME",
        )

    def test_12(self):
        self.assertEqual(
            loves_me(12),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, "
            "Loves me not, Loves me, LOVES ME NOT",
        )

    def test_13(self):
        self.assertEqual(
            loves_me(13),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, "
            "Loves me not, Loves me, Loves me not, LOVES ME",
        )

    def test_14(self):
        self.assertEqual(
            loves_me(14),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, "
            "Loves me not, Loves me, Loves me not, Loves me, LOVES ME NOT",
        )

    def test_15(self):
        self.assertEqual(
            loves_me(15),
            "Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, Loves me not, Loves me, "
            "Loves me not, Loves me, Loves me not, Loves me, Loves me not, LOVES ME",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Loves Me, Loves Me Not...](https://edabit.com/challenge/6pEGXsuCAxbWTRkgc)
