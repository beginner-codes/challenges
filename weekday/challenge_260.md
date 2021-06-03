# Challenge 260 - Number of Apples Left

A man has a bunch of apples. If he eats a percentage of the apples, his children will share the remainder of the apples. Create a function to determine the number of whole apples his children get. If his children do not get any apples, return `"The children didn't get any apples"`.

## Examples
```python
get_number_of_apples(10, "90%") ➞ 1

get_number_of_apples(25, "10%") ➞ 22

get_number_of_apples(0, "10%") ➞ "The children didn't get any apples"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def get_number_of_apples(apples: int, eaten: str) -> int:
    return 0  # Put your code here!!!`


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(get_number_of_apples(10, "90%"), 1)

    def test_2(self):
        self.assertEqual(get_number_of_apples(25, "10%"), 22)

    def test_3(self):
        self.assertEqual(
            get_number_of_apples(0, "10%"), "The children didn't get any apples"
        )

    def test_4(self):
        self.assertEqual(get_number_of_apples(40, "30%"), 28)

    def test_5(self):
        self.assertEqual(get_number_of_apples(10, "44%"), 5)

    def test_6(self):
        self.assertEqual(
            get_number_of_apples(12, "100%"), "The children didn't get any apples"
        )

    def test_7(self):
        self.assertEqual(
            get_number_of_apples(40, "100%"), "The children didn't get any apples"
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Number of Apples Left](https://edabit.com/challenge/wvPTPAqARjE9fswCE)
