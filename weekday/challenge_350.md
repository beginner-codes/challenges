# Challenge 350 - Capitalize the Last Letter

Create a function that capitalizes the last letter of every word.

## Examples
```python
cap_last("hello") ➞ "hellO"

cap_last("My Name Is Beginner Codes") ➞ "MY NamE IS BeginneR CodeS"

cap_last("HELp THe LASt LETTERs CAPITALISe") ➞ "HELP THE LAST LETTERS CAPITALISE"
```
## Notes

- There won't be any cases of punctuation in the tests.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def cap_last(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(cap_last("hello"), "hellO")

    def test_2(self):
        self.assertEqual(cap_last("My Name Is Beginner Codes"), "MY NamE IS BeginneR CodeS")

    def test_3(self):
        self.assertEqual(
            cap_last("HELp THe LASt LETTERs CAPITALISe"),
            "HELP THE LAST LETTERS CAPITALISE",
        )

    def test_4(self):
        self.assertEqual(cap_last("hellooooo"), "hellooooO")

    def test_5(self):
        self.assertEqual(
            cap_last("hahA I aM alreadY capitaliseD"), "hahA I aM alreadY capitaliseD"
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Capitalize the Last Letter](https://edabit.com/challenge/vAwDW47yngWh8iMwN)
