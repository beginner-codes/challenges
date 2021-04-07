# Challenge 220 - Capital Split

Create a function which adds spaces before every capital in a word. Uncapitalize the whole string afterwards.

## Examples
```python
cap_space("helloWorld") ➞ "hello world"

cap_space("iLoveMyTeapot") ➞ "i love my teapot"

cap_space("stayIndoors") ➞ "stay indoors"
```
## Notes

- The first letter will stay uncapitalized.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def cap_space(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(cap_space("helloWorld"), "hello world")

    def test_2(self):
        self.assertEqual(cap_space("iLoveMyTeapot"), "i love my teapot")

    def test_3(self):
        self.assertEqual(cap_space("stayIndoors"), "stay indoors")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Capital Split](https://edabit.com/challenge/riF3RkrcKpBp3sKCX)
