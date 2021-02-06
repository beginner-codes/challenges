# Challenge 179 - Goldbach's Weak Conjecture

According to Goldbach’s weak conjecture, every odd number greater than `5` can be expressed as the sum of three prime numbers. (A prime may be used more than once in the same sum.) This conjecture is called "weak" because if Goldbach's strong conjecture (concerning sums of two primes) is proven, it would be true. Computer searches have only reached as far as 1018 for the strong Goldbach conjecture, and not much further than that for the weak Goldbach conjecture.

Your task today is to write a program that applies Goldbach's weak conjecture to numbers and shows which 3 primes, added together, yield the result.

Your program should emit three prime numbers (remember, one may be used multiple times) to yield the target sum.

## Example
```py
goldbachs_conjecture(11) -> (3, 3, 5)
goldbachs_conjecture(35) -> (19, 13, 3)
```

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
from __future__ import annotations
import unittest


def goldbachs_conjecture(number: int) -> tuple[int, int, int]:
    return 0, 0, 0


class Test(unittest.TestCase):
    def test_1(self):
        self.assertEqual(goldbachs_conjecture(11), (3, 3, 5))

    def test_2(self):
        self.assertEqual(goldbachs_conjecture(35), (19, 13, 3))


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on r/dailyprogrammer: [\[2018-04-11\] Challenge #356 \[Intermediate\] Goldbach's Weak Conjecture
](https://www.reddit.com/r/dailyprogrammer/comments/8bh8dh/20180411_challenge_356_intermediate_goldbachs/)

