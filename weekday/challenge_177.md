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


def reversible_inclusive_list(start: int, end: int) -> list[int]:
    return []  # Put your code here!!!


class Test(unittest.TestCase):
    def test_1(self):
        self.assertEqual(reversible_inclusive_list(5, 1), [5, 4, 3, 2, 1])

    def test_2(self):
        self.assertEqual(reversible_inclusive_list(6, 2), [6, 5, 4, 3, 2])

    def test_3(self):
        self.assertEqual(
            reversible_inclusive_list(10, 20),
            [10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20],
        )

    def test_4(self):
        self.assertEqual(
            reversible_inclusive_list(24, 17), [24, 23, 22, 21, 20, 19, 18, 17]
        )

    def test_5(self):
        self.assertEqual(
            reversible_inclusive_list(40, 50),
            [40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50],
        )

    def test_6(self):
        self.assertEqual(
            reversible_inclusive_list(51, 41),
            [51, 50, 49, 48, 47, 46, 45, 44, 43, 42, 41],
        )

    def test_7(self):
        self.assertEqual(
            reversible_inclusive_list(11, 66),
            [
                11,
                12,
                13,
                14,
                15,
                16,
                17,
                18,
                19,
                20,
                21,
                22,
                23,
                24,
                25,
                26,
                27,
                28,
                29,
                30,
                31,
                32,
                33,
                34,
                35,
                36,
                37,
                38,
                39,
                40,
                41,
                42,
                43,
                44,
                45,
                46,
                47,
                48,
                49,
                50,
                51,
                52,
                53,
                54,
                55,
                56,
                57,
                58,
                59,
                60,
                61,
                62,
                63,
                64,
                65,
                66,
            ],
        )

    def test_8(self):
        self.assertEqual(reversible_inclusive_list(9, 3), [9, 8, 7, 6, 5, 4, 3])

    def test_9(self):
        self.assertEqual(
            reversible_inclusive_list(6, 16), [6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16]
        )


if __name__ == "__main__":
    unittest.main()

```
## Credits

Found on Edabit: [Reversible Inclusive List Ranges](https://edabit.com/challenge/zW9JME7XNew4tgCCE)

