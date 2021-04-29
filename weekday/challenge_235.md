# Challenge 235 - Transcribe to mRNA

Transcribe the given DNA strand into corresponding mRNA - a type of RNA, that will be formed from it after transcription. DNA has the bases A, T, G and C, while RNA converts to U, A, C and G respectively.

## Examples
```python
dna_to_rna("ATTAGCGCGATATACGCGTAC") ➞ "UAAUCGCGCUAUAUGCGCAUG"

dna_to_rna("CGATATA") ➞ "GCUAUAU"

dna_to_rna("GTCATACGACGTA") ➞ "CAGUAUGCUGCAU"
```
## Notes

- Transcription is the process of making complementary strand.
- A, T, G and C in DNA converts to U, A, C and G respectively, when in mRNA.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def dna_to_rna(dna: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(dna_to_rna("GCGTAC"), "CGCAUG")

    def test_2(self):
        self.assertEqual(dna_to_rna("ATTAGCGCGATATACGCGTAC"), "UAAUCGCGCUAUAUGCGCAUG")

    def test_3(self):
        self.assertEqual(dna_to_rna("CAGTATGCTGCAT"), "GUCAUACGACGUA")

    def test_4(self):
        self.assertEqual(dna_to_rna("CGATATA"), "GCUAUAU")

    def test_5(self):
        self.assertEqual(dna_to_rna("GCAGCTACA"), "CGUCGAUGU")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Transcribe to mRNA](https://edabit.com/challenge/McZF4JRhPus5DtRA4)
