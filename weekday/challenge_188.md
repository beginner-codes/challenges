# Challenge 188 - The Ducci Sequence

A Ducci sequence is a sequence of n-tuples of integers, sometimes known as "the Diffy game", because it is based on sequences. Given an n-tuple of integers `(a_1, a_2, ... a_n)` the next n-tuple in the sequence is formed by taking the absolute differences of neighboring integers. Ducci sequences are named after Enrico Ducci (1864-1940), the Italian mathematician credited with their discovery.

Some Ducci sequences descend to all zeroes or a repeating sequence. An example is `(1,2,1,2,1,0)` -> `(1,1,1,1,1,1)` -> `(0,0,0,0,0,0)`.

Additional information about the Ducci sequence can be found in this writeup from Greg Brockman, a mathematics student. http://www.cut-the-knot.org/Curriculum/Algebra/GregBrockman/GregBrockmanDucciSequences.shtml

It's kind of fun to play with the code once you get it working and to try and find sequences that never collapse and repeat. One I found was `(2, 4126087, 4126085)`, it just goes on and on.

It's also kind of fun to plot these in 3 dimensions. Here is an example of the sequence `(129,12,155,772,63,4)` turned into 2 sets of lines `(x1, y1, z1, x2, y2, z2)`. https://monkey.org/~jose/graphing/ducci/index2.html

## Input Description

You'll be given an n-tuple, one per line. Example:
```python
(0, 653, 1854, 4063)
```
## Output Description

Your program should emit the number of steps taken to get to either an all 0 tuple or when it enters a stable repeating pattern.

## Example
```
[0; 653; 1854; 4063]
[653; 1201; 2209; 4063]
[548; 1008; 1854; 3410]
[460; 846; 1556; 2862]
[386; 710; 1306; 2402]
[324; 596; 1096; 2016]
[272; 500; 920; 1692]
[228; 420; 772; 1420]
[192; 352; 648; 1192]
[160; 296; 544; 1000]
[136; 248; 456; 840]
[112; 208; 384; 704]
[96; 176; 320; 592]
[80; 144; 272; 496]
[64; 128; 224; 416]
[64; 96; 192; 352]
[32; 96; 160; 288]
[64; 64; 128; 256]
[0; 64; 128; 192]
[64; 64; 64; 192]
[0; 0; 128; 128]
[0; 128; 0; 128]
[128; 128; 128; 128]
[0; 0; 0; 0]
24 steps
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
from __future__ import annotations
import unittest


def ducci_sequence(sequence: tuple[int, ...]) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(ducci_sequence((1, 5, 7, 9, 9)), 23)

    def test_2(self):
        self.assertEqual(ducci_sequence((1, 2, 1, 2, 1, 0)), 3)

    def test_3(self):
        self.assertEqual(ducci_sequence((10, 12, 41, 62, 31, 50)), 22)

    def test_4(self):
        self.assertEqual(ducci_sequence((10, 12, 41, 62, 31)), 30)

    def test_5(self):
        self.assertEqual(ducci_sequence((0, 653, 1854, 4063)), 24)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on /r/dailyprogrammer: [[2018-06-20\] Challenge #364 \[Intermediate\] The Ducci Sequence](https://www.reddit.com/r/dailyprogrammer/comments/8sjcl0/20180620_challenge_364_intermediate_the_ducci/)
