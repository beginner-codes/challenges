# Challenge 176 - CAPS LOCK DAY is over!

Yesterday was CAPS LOCK DAY. Apart from that day, every sentence should be lowercase, so write a function to normalize a sentence.

Create a function that takes a string. If the string is all uppercase characters, convert it to lowercase and add an exclamation mark at the end.

## Examples
```py
normalize("CAPS LOCK DAY IS OVER") ➞ "Caps lock day is over!"

normalize("Today is not caps lock day.") ➞ "Today is not caps lock day."

normalize("Let us stay calm, no need to panic.") ➞ "Let us stay calm, no need to panic."
```
## Notes

- Each string is a sentence and should start with an uppercase character.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **Join us on Discord!!!**

[beginner.py](https://discord.gg/sfHykntuGy)

## Challenge Tests
```py
import unittest


def normalize(text: str) -> str:
    return ""  # Put your code here!!!


class Test(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            normalize("CAPS LOCK DAY IS OVER"),
            "Caps lock day is over!",
        )

    def test_2(self):
        self.assertEqual(
            normalize("Today is not caps lock day."), "Today is not caps lock day."
        )

    def test_3(self):
        self.assertEqual(
            normalize("WE WANT THIS COVID THING TO BE OVER"),
            "We want this covid thing to be over!",
        )

    def test_4(self):
        self.assertEqual(
            normalize("Let us stay calm, no need to panic."),
            "Let us stay calm, no need to panic.",
        )

    def test_5(self):
        self.assertEqual(normalize("DO NOT SHOUT"), "Do not shout!")

    def test_6(self):
        self.assertEqual(
            normalize("Civilized conversation."), "Civilized conversation."
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [CAPS LOCK DAY is over!](https://edabit.com/challenge/aqA6KSHRCwfE44Q9m)

