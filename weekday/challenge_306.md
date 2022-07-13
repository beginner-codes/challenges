# Challenge 306 - Scottish Screaming

A strong Scottish accent makes every vowel similar to an "e", so you should replace every vowel with an "e". Additionally, it is being screamed, so it should be in block capitals.

Create a function that takes a string and returns a string.

## Examples
```python
to_scottish_screaming("hello world") ➞ "HELLE WERLD"

to_scottish_screaming("Mr. Fox was very naughty") ➞ "MR. FEX WES VERY NEEGHTY"

to_scottish_screaming("Butterflies are beautiful!") ➞ "BETTERFLEES ERE BEEETEFEL!"
```
## Notes

- Make sure to include all punctuation that is in the original string.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def to_scottish_screaming(phrase: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(to_scottish_screaming("lorem ipsum"), "LEREM EPSEM")

    def test_2(self):
        self.assertEqual(to_scottish_screaming("Leeroy jenkins!"), "LEEREY JENKENS!")

    def test_3(self):
        self.assertEqual(
            to_scottish_screaming("A, wonderful, day, don't, you, think?"),
            "E, WENDERFEL, DEY, DEN'T, YEE, THENK?",
        )

    def test_4(self):
        self.assertEqual(to_scottish_screaming("Hello world"), "HELLE WERLD")

    def test_5(self):
        self.assertEqual(
            to_scottish_screaming("start queueing you oafs"), "STERT QEEEEENG YEE EEFS"
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Scottish Screaming](https://edabit.com/challenge/2hvruws6kgiKj98Rv)
