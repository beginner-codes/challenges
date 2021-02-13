# Challenge 183 - Catching Car Mileage Numbers

> "7777...8?!??!", exclaimed Bob, "I missed it again! Argh!" Every time there's an interesting number coming up, he notices and then promptly forgets. Who doesn't like catching those one-off interesting mileage numbers?

Let's make it so Bob never misses another interesting number. We've hacked into his car's computer, and we have a box hooked up that reads mileage numbers. We've got a box glued to his dash that lights up yellow or green depending on whether it receives a 1 or a 2 (respectively).

It's up to you, intrepid warrior, to glue the parts together. Write the function that parses the mileage number input, and returns a 2 if the number is "interesting" (see below), a 1 if an interesting number occurs within the next two miles, or a 0 if the number is not interesting.

## "Interesting" Numbers
Interesting numbers are 3-or-more digit numbers that meet one or more of the following criteria:

- Any digit followed by all zeros: 100, 90000
- Every digit is the same number: 1111
- The digits are sequential, incementing†: 1234
- The digits are sequential, decrementing‡: 4321
- The digits are a palindrome: 1221 or 73837

*† For incrementing sequences, 0 should come after 9, and not before 1, as in 7890.*
*‡ For decrementing sequences, 0 should come after 1, and not before 9, as in 3210.*

So, you should expect these inputs and outputs:
```py
# "boring" numbers
is_interesting(3)    # 0
is_interesting(3236) # 0

# progress as we near an "interesting" number
is_interesting(11207, []) # 0
is_interesting(11208, []) # 0
is_interesting(11209, []) # 1
is_interesting(11210, []) # 1
is_interesting(11211, []) # 2
```
## Error Checking

- A number is only interesting if it is greater than 99!
- Input will always be an integer greater than 0, and less than 1,000,000,000.
- You should only ever output 0, 1, or 2.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```py
import unittest


def is_interesting(mileage: int) -> int:
    return 0  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(is_interesting(3), 0)

    def test_2(self):
        self.assertEqual(is_interesting(11208), 0)

    def test_3(self):
        self.assertEqual(is_interesting(11209), 1)

    def test_4(self):
        self.assertEqual(is_interesting(11211), 2)

    def test_5(self):
        self.assertEqual(is_interesting(90000), 2)

    def test_6(self):
        self.assertEqual(is_interesting(89999), 1)

    def test_7(self):
        self.assertEqual(is_interesting(59998), 1)

    def test_8(self):
        self.assertEqual(is_interesting(59997), 0)

    def test_9(self):
        self.assertEqual(is_interesting(7890), 2)

    def test_10(self):
        self.assertEqual(is_interesting(7889), 1)

    def test_11(self):
        self.assertEqual(is_interesting(7888), 1)

    def test_12(self):
        self.assertEqual(is_interesting(1231), 0)

    def test_13(self):
        self.assertEqual(is_interesting(3210), 2)

    def test_14(self):
        self.assertEqual(is_interesting(12321), 2)

    def test_15(self):
        self.assertEqual(is_interesting(12320), 1)

    def test_16(self):
        self.assertEqual(is_interesting(12319), 1)

    def test_17(self):
        self.assertEqual(is_interesting(12318), 0)


if __name__ == "__main__":
    unittest.main()
```
## Credits

Adapted from CodeWars: [Catching Car Mileage Numbers](https://www.codewars.com/kata/52c4dd683bfd3b434c000292/train/python)
