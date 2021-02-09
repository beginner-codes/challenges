# Challenge 180 - H4ck3r Sp34k

Create a function that takes a string as an argument and returns a coded (h4ck3r 5p34k) version of the string.

## Examples
```python
hacker_speak("javascript is cool") ➞ "j4v45cr1pt 15 c00l"

hacker_speak("programming is fun") ➞ "pr0gr4mm1ng 15 fun"

hacker_speak("become a coder") ➞ "b3c0m3 4 c0d3r"
```
## Notes

- In order to work properly, the function should replace all `"a"`s with 4, `"e"`s with 3, `"i"`s with 1, `"o"`s with 0, and `"s"`s with 5.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
import unittest


def hacker_speak(text: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(hacker_speak("javascript is cool"), "j4v45cr1pt 15 c00l")

    def test_2(self):
        self.assertEqual(hacker_speak("become a coder"), "b3c0m3 4 c0d3r")

    def test_3(self):
        self.assertEqual(hacker_speak("hi there"), "h1 th3r3")

    def test_4(self):
        self.assertEqual(hacker_speak("programming is fun"), "pr0gr4mm1ng 15 fun")

    def test_5(self):
        self.assertEqual(hacker_speak("keep on practicing"), "k33p 0n pr4ct1c1ng")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [H4ck3r Sp34k](https://edabit.com/challenge/nPdPSgSsGfdyRbHkd)
