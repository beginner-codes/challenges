# Challenge 177 - Reversible Inclusive List Ranges!

Write a function that, given the `start_of_range` and `end_of_range` values, returns a list containing all the numbers inclusive to that range.

## Examples
```python
reversible_inclusive_list(1, 5) ➞ [1, 2, 3, 4, 5]

reversible_inclusive_list(2, 8) ➞ [2, 3, 4, 5, 6, 7, 8]

reversible_inclusive_list(10, 20) ➞ [10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]

reversible_inclusive_list(24, 17) ➞ [24, 23, 22, 21, 20, 19, 18, 17]
```
## Notes

- The sort order of the resulting array is dependent of the input values.
- All inputs provided in the test scenarios are valid.
- If `start_of_range` is greater than `end_of_range`, return a list in descending order, otherwise, ascending order.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

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

Found on Edabit: [Reversible Inclusive List Ranges](https://edabit.com/challenge/zW9JME7XNew4tgCCE)

