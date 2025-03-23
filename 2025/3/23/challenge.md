# The Forgotten Glyphs of Orion-9
-# March 23rd, 2025

In the year 3127, deep in the Andromeda Cluster, an ancient starship known as the Orion-9 drifts silently through the void. It was once the pride of the Galactic Empire, but centuries ago, it vanished without a trace.

You and your team of cyber-archaeologists have awakened the derelict vessel's dormant systems, searching for clues to its fate.

In the ship’s central databank, you discover encrypted logs—categorized using a strange, archaic code. At first, it looks like nonsense, but then your AI assistant chimes in:

“These symbols… they resemble an ancient Earth numbering system. Roman numerals. If we can decode them, we might find a way to uncover what happened to the Orion-9.”

**Your task**: Convert the encoded Roman numeral sequences into standard numbers to help unlock the secrets of the Orion-9.

*Roman Numerals:*

```
I        1
V        5
X       10
L       50
C      100
D      500
M    1,000
```

You'll be given a Roman Numeral, return the corresponding integer.

```python
decode_numerals("IV") ➞ 4

decode_numerals("XIX") ➞ 19

decode_numerals("MMVIII") ➞ 2008
```

## Test Cases

You can download test cases with this command:

```shell
curl https://raw.githubusercontent.com/beginner-codes/challenges/refs/heads/main/2025/3/23/test_cases.json > 20250323_test_cases.json
```

They're stored as JSON using this schema:

```json
[
  {
    "parameters": ["XIX"],
    "expected_result": "19"
  },
  ...
]
``` 

The expected result is always stringified to allow for results that may exceed the bounds of an integer.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**