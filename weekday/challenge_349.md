# Challenge 349 - Remove Repeated Letters

Create a function that replaces all consecutively repeated letters in a word with single letters.

## Examples
```python
remove_repeats("aaabbbccc") ➞ "abc"

remove_repeats("bookkeeper") ➞ "bokeper"

remove_repeats("nananana") ➞ "nananana"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def remove_repeats(string: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(remove_repeats("aaabbbccc"), "abc")

    def test_2(self):
        self.assertEqual(remove_repeats("bookkeeper"), "bokeper")

    def test_3(self):
        self.assertEqual(remove_repeats("nananana"), "nananana")

    def test_4(self):
        self.assertEqual(
            remove_repeats("accddbccabadcabccdababaacbdaadcccbcaabaaddbabbaadd"),
            "acdbcabadcabcdababacbdadcbcabadbabad",
        )

    def test_5(self):
        self.assertEqual(
            remove_repeats("aabbcabdcddddacdccacbbcabadccbbaadcccbddacbdbabbbd"),
            "abcabdcdacdcacbcabadcbadcbdacbdbabd",
        )

    def test_6(self):
        self.assertEqual(
            remove_repeats("dacbaabacbabacabcabaabdccccbdbbcaadddacdbdbdacbada"),
            "dacbabacbabacabcababdcbdbcadacdbdbdacbada",
        )

    def test_7(self):
        self.assertEqual(
            remove_repeats("cbdbcbcccbdbbcaaaacacbcabddcdcddcccbdaabdacbdcabbd"),
            "cbdbcbcbdbcacacbcabdcdcdcbdabdacbdcabd",
        )

    def test_8(self):
        self.assertEqual(
            remove_repeats("cdbdcdccccbcbbcdabbbbcababccadccabdcacabbcaccdaccd"),
            "cdbdcdcbcbcdabcababcadcabdcacabcacdacd",
        )

    def test_9(self):
        self.assertEqual(
            remove_repeats("bacbdbdadbbbdacbddbdcbadddabbaadcbbdabdaabcdddbacd"),
            "bacbdbdadbdacbdbdcbadabadcbdabdabcdbacd",
        )

    def test_10(self):
        self.assertEqual(
            remove_repeats("daadadccbcacacbacdbbaabaadbaabadacdacadbacdcababbb"),
            "dadadcbcacacbacdbabadbabadacdacadbacdcabab",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Remove Repeated Letters](https://edabit.com/challenge/3Eia4oLLCcyyLN2L7)
