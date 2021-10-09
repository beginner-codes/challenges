# Challenge 352 - Underscore-Hash Staircase

Create a function that will build a staircase using the underscore `_` and hash `#` symbols. A positive value denotes the staircase's upward direction and downwards for a negative value.

## Examples
```python
staircase(3) ➞ "__#\n_##\n###"
__#
_##
###

staircase(7) ➞ "______#\n_____##\n____###\n___####\n__#####\n_######\n#######"
______#
_____##
____###
___####
__#####
_######
#######

staircase(2) ➞ "_#\n##"
_#
##

staircase(-8) ➞ "########\n_#######\n__######\n___#####\n____####\n_____###\n______##\n_______#"
########
_#######
__######
___#####
____####
_____###
______##
_______#
```
## Notes

- All inputs are either positive or negative values.
- The string to be returned is adjoined with the newline character (`\n`).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def staircase(steps: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(staircase(3), "__#\n_##\n###")

    def test_2(self):
        self.assertEqual(
            staircase(7),
            "______#\n_____##\n____###\n___####\n__#####\n_######\n#######",
        )

    def test_3(self):
        self.assertEqual(staircase(2), "_#\n##")

    def test_4(self):
        self.assertEqual(
            staircase(-8),
            "########\n_#######\n__######\n___#####\n____####\n_____###\n______##\n_______#",
        )

    def test_5(self):
        self.assertEqual(staircase(4), "___#\n__##\n_###\n####")

    def test_6(self):
        self.assertEqual(
            staircase(-12),
            "############\n_###########\n__##########\n___#########\n____########\n_____#######\n______######\n_______#####\n________####\n_________###\n__________##\n___________#",
        )

    def test_7(self):
        self.assertEqual(
            staircase(11),
            "__________#\n_________##\n________###\n_______####\n______#####\n_____######\n____#######\n___########\n__#########\n_##########\n###########",
        )

    def test_8(self):
        self.assertEqual(
            staircase(-6), "######\n_#####\n__####\n___###\n____##\n_____#"
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Underscore-Hash Staircase](https://edabit.com/challenge/YqLBEZJR9ySndYQpH)
