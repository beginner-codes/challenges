# Challenge 394 - RNA Reverse Complement

Create a function that finds the reverse complement of a ribonucleic acid (RNA) strand. The RNA will be represented as a string containing only the characters `"A"`, `"C"`, `"G"`, and `"U"`. Since RNA can only (canonically) allow pairings of A/U and G/C, the complement of an RNA would be as follows:
```
original -> complement
"AAA" -> "UUU"
"UUU" -> "AAA"
"GGG" -> "CCC"
"CCC" -> "GGG"
"GGAACC" -> "CCUUGG"
```
Your function should find the complement on the right AND also reverse the resulting string.

## Examples
```python
reverse_complement("GUGU") ➞ "ACAC"

reverse_complement("UCUCG") ➞ "CGAGA"

reverse_complement("CAGGU") ➞ "ACCUG"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


def reverse_complement(rna: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(reverse_complement("GAGGC"), "GCCUC")

    def test_2(self):
        self.assertEqual(reverse_complement("UCUCG"), "CGAGA")

    def test_3(self):
        self.assertEqual(reverse_complement("CAGGU"), "ACCUG")

    def test_4(self):
        self.assertEqual(reverse_complement("UAUUUUUCCA"), "UGGAAAAAUA")

    def test_5(self):
        self.assertEqual(reverse_complement("GUAGGCAACA"), "UGUUGCCUAC")

    def test_6(self):
        self.assertEqual(reverse_complement("UAGCUAAAUC"), "GAUUUAGCUA")

    def test_7(self):
        self.assertEqual(reverse_complement("AUGAGCGUAC"), "GUACGCUCAU")

    def test_8(self):
        self.assertEqual(
            reverse_complement("UUAUACCCGAGUCGGAUUUGUCACU"), "AGUGACAAAUCCGACUCGGGUAUAA"
        )

    def test_9(self):
        self.assertEqual(
            reverse_complement("CUUGUGCGCUAUACAUCGAGUAGUUGCUAGAGUAUGUUACUCAAGAGCGC"),
            "GCGCUCUUGAGUAACAUACUCUAGCAACUACUCGAUGUAUAGCGCACAAG",
        )

    def test_10(self):
        self.assertEqual(
            reverse_complement(
                "UUAACUGGGGUGAACUGUCCUGAGCCUAUGGAUCUGCGCGCAGGGCUUCAAAUGGAGUUCGGAAUGACCAUCGAUUCUCGAUGUUUGGCACGAAGUCGCA"
            ),
            "UGCGACUUCGUGCCAAACAUCGAGAAUCGAUGGUCAUUCCGAACUCCAUUUGAAGCCCUGCGCGCAGAUCCAUAGGCUCAGGACAGUUCACCCCAGUUAA",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [RNA Reverse Complement](https://edabit.com/challenge/DGK42TmQiocZqifxi)
