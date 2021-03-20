# Challenge 207 - Parentheses Clusters

Write a function that groups a string into parentheses cluster. Each cluster should be balanced.

## Examples
```python
split("()()()") ➞ ["()", "()", "()"]

split("((()))") ➞ ["((()))"]

split("((()))(())()()(()())") ➞ ["((()))", "(())", "()", "()", "(()())"]

split("((())())(()(()()))") ➞ ["((())())", "(()(()()))"]
```
## Notes

- All input strings will only contain parentheses.
- Balanced: Every opening parens ( must exist with its matching closing parens ) in the same cluster.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def split(parentheses: str) -> list[str]:
    return []  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(split("()()()"), ["()", "()", "()"])

    def test_2(self):
        self.assertEqual(split(""), [])

    def test_3(self):
        self.assertEqual(split("()()(())"), ["()", "()", "(())"])

    def test_4(self):
        self.assertEqual(split("(())(())"), ["(())", "(())"])

    def test_5(self):
        self.assertEqual(split("((()))"), ["((()))"])

    def test_6(self):
        self.assertEqual(
            split("()(((((((((())))))))))"), ["()", "(((((((((())))))))))"]
        )

    def test_7(self):
        self.assertEqual(
            split("((())()(()))(()(())())(()())"),
            ["((())()(()))", "(()(())())", "(()())"],
        )

    def test_8(self):
        self.assertEqual(
            split("((()))(())()()(()())"), ["((()))", "(())", "()", "()", "(()())"]
        )

    def test_9(self):
        self.assertEqual(split("((())())(()(()()))"), ["((())())", "(()(()()))"])

    def test_10(self):
        self.assertEqual(
            split("(()(()()))()(((()))()(()))(()((()))(())())"),
            ["(()(()()))", "()", "(((()))()(()))", "(()((()))(())())"],
        )
```
## Credits

Found on Edabit: [Parentheses Clusters](https://edabit.com/challenge/Fpymv2HieqEd7ptAq)
