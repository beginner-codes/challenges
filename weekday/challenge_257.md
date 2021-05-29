# Challenge 257 - Primal Strength

In number theory, a prime number is balanced if it is equidistant from the prime before it and the prime after it. It is therefore the arithmetic mean of those primes. For example, 5 is a balanced prime, two units away from 3, and two from 7. 211 is 12 units away from the previous prime, 199, and 12 away from the next, 223.

A prime that is greater than the arithmetic mean of the primes before and after it is called a strong prime. It is closer to the prime after it than the one before it. For example, the strong prime 17 is closer to 19 than it is to 13.

A prime that is lesser than the arithmetic mean of the primes before and after it is called weak prime. For example, 19.

Create a function that takes a prime number as input and returns `"Strong"` if it is a strong prime, `"Weak"` if it is a weak prime, or `"Balanced"`.

## Examples
```python
primal_strength(211) ➞ "Balanced"

primal_strength(17) ➞ "Strong"

primal_strength(19) ➞ "Weak"
```
## Notes

- This definition of strong primes is not to be confused with strong primes as defined in cryptography, which are much more complicated than this. You are all welcome to make a challenge based on cryptographically strong primes.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def primal_strength(prime: int) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(primal_strength(5), "Balanced")

    def test_2(self):
        self.assertEqual(primal_strength(211), "Balanced")

    def test_3(self):
        self.assertEqual(primal_strength(593), "Balanced")

    def test_4(self):
        self.assertEqual(primal_strength(1693), "Strong")

    def test_5(self):
        self.assertEqual(primal_strength(599), "Strong")

    def test_6(self):
        self.assertEqual(primal_strength(2203), "Strong")

    def test_7(self):
        self.assertEqual(primal_strength(19), "Weak")

    def test_8(self):
        self.assertEqual(primal_strength(2971), "Weak")

    def test_9(self):
        self.assertEqual(primal_strength(1493), "Weak")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Primal Strength](https://edabit.com/challenge/n3w4fqdaMuCB9bjgs)
