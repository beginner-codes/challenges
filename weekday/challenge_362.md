# Challenge 362 - Longest Alternating Substring

Given a string of digits, write a function that returns the longest substring with alternating odd/even or even/odd digits. If two or more substrings have the same length, return the substring that occurs first.

## Examples
```python
longest_substring("225424272163254474441338664823") ➞ "272163254"
# substrings = 254, 272163254, 474, 41, 38, 23

longest_substring("594127169973391692147228678476") ➞ "16921472"
# substrings = 94127, 169, 16921472, 678, 476

longest_substring("721449827599186159274227324466") ➞ "7214"
# substrings = 7214, 498, 27, 18, 61, 9274, 27, 32
# 7214 and 9274 have same length, but 7214 occurs first.
```
## Notes

- The minimum alternating substring size is `2`.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def longest_substring(digits: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(longest_substring("844929328912985315632725682153"), "56327256")

    def test_2(self):
        self.assertEqual(longest_substring("769697538272129475593767931733"), "27212947")

    def test_3(self):
        self.assertEqual(longest_substring("937948289456111258444958189244"), "894561")

    def test_4(self):
        self.assertEqual(longest_substring("736237766362158694825822899262"), "636")

    def test_5(self):
        self.assertEqual(longest_substring("369715978955362655737322836233"), "369")

    def test_6(self):
        self.assertEqual(longest_substring("345724969853525333273796592356"), "496985")

    def test_7(self):
        self.assertEqual(longest_substring("548915548581127334254139969136"), "8581")

    def test_8(self):
        self.assertEqual(longest_substring("417922164857852157775176959188"), "78521")

    def test_9(self):
        self.assertEqual(longest_substring("251346385699223913113161144327"), "638569")

    def test_10(self):
        self.assertEqual(longest_substring("483563951878576456268539849244"), "18785")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Longest Alternating Substring](https://edabit.com/challenge/RB6iWFrCd6rXWH3vi)
