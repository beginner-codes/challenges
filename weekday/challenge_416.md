# Challenge 416 - ASCII Art!

Given a very long string of ASCII characters, split the string up into equal sized groups of size width. To properly display the image, join up the groups with the newline character `\n` and return the output string.

See the miniature examples below for clarity!

## Examples
```python
format_ascii("0123456789", 2) ➞ "01\n23\n45\n67\n89"

format_ascii("................................", 8) ➞ "........\n........\n........\n........"

format_ascii("^^^^^^^^", 1) ➞ "^\n^\n^\n^\n^\n^\n^\n^"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def format_ascii(text: str, wrap_width: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(format_ascii("#@#@#@#@", 2), "#@\n#@\n#@\n#@")

    def test_2(self):
        self.assertEqual(format_ascii("0123456789", 2), "01\n23\n45\n67\n89")

    def test_3(self):
        self.assertEqual(
            format_ascii("................................", 8),
            "........\n........\n........\n........",
        )

    def test_4(self):
        self.assertEqual(format_ascii("^^^^^^^^", 1), "^\n^\n^\n^\n^\n^\n^\n^")

    def test_5(self):
        art1 = (
            "                                                  \n"
            "                 ....,,,,,,,,....                 \n"
            "               .,,,,,,,,,,,,,,,,,,.               \n"
            "             .,,........,,,,,,,,,,,,.             \n"
            "            .,.....:*,.,,,,,:?:,,,,,,,            \n"
            "           .,......S@*.,,,,,%@?,,,,,,,,           \n"
            "          .,.......S@*.,,,,,%@?,,,,,,.,.          \n"
            "          .........:*,.,,,,,:?:,,,,,,.,,          \n"
            "          .............,,,,,,,,,,,,,,.,,          \n"
            "          .,....,:......,,,,,,,.:;,,,.,.          \n"
            "          .,,...,??:.........,:*%;,,,,,.          \n"
            "           .,,,,,,+%S?+;;;;+?SS*,,,,,,.           \n"
            "            ..,,,,,,;*%SSSS%?;,,,,,,..            \n"
            "              ..,,,,,,,,,,,,,,::,,..              \n"
            "                 ...,,,,,,,,,,,..                 \n"
            "                     ........                     "
        )
        self.assertEqual(
            format_ascii(
                "                                                                   ....,,,,,,,,....                   "
                "             .,,,,,,,,,,,,,,,,,,.                            .,,........,,,,,,,,,,,,.                 "
                "        .,.....:*,.,,,,,:?:,,,,,,,                       .,......S@*.,,,,,%@?,,,,,,,,                 "
                "    .,.......S@*.,,,,,%@?,,,,,,.,.                    .........:*,.,,,,,:?:,,,,,,.,,                  "
                "  .............,,,,,,,,,,,,,,.,,                    .,....,:......,,,,,,,.:;,,,.,.                    "
                ".,,...,??:.........,:*%;,,,,,.                     .,,,,,,+%S?+;;;;+?SS*,,,,,,.                       "
                "..,,,,,,;*%SSSS%?;,,,,,,..                          ..,,,,,,,,,,,,,,::,,..                            "
                "   ...,,,,,,,,,,,..                                      ........                     ",
                50,
            ),
            art1,
        )

        
if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [ASCII Art!](https://edabit.com/challenge/G7m26EdX3AABCSQBv)
