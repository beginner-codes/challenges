# Challenge 293 - Making a Countdown

Create a function where given the number to count down from, and a phrase to say, return a countdown sequence as a string leading up to the words at the end.

Put a full stop after each number and uppercase and add an exclamation mark to the phrase. See the examples below for clarification!

## Examples
```python
countdown(10, "Blast Off") ➞ "10. 9. 8. 7. 6. 5. 4. 3. 2. 1. BLAST OFF!"

countdown(3, "go") ➞ "3. 2. 1. GO!"

countdown(5, "FIRE") ➞ "5. 4. 3. 2. 1. FIRE!"
```
## Notes

- `start_at` will be a number greater than `0`.
- The phrase will need the exclamation mark.
- Don't include `0` in the countdown.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
import unittest


def countdown(start_at: int, say: str) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    def test_1(self):
        self.assertEqual(
            countdown(10, "Blast Off"), "10. 9. 8. 7. 6. 5. 4. 3. 2. 1. BLAST OFF!"
        )

    def test_2(self):
        self.assertEqual(countdown(3, "go"), "3. 2. 1. GO!")

    def test_3(self):
        self.assertEqual(countdown(5, "FIRE"), "5. 4. 3. 2. 1. FIRE!")

    def test_4(self):
        self.assertEqual(
            countdown(12, "watch out"),
            "12. 11. 10. 9. 8. 7. 6. 5. 4. 3. 2. 1. WATCH OUT!",
        )

    def test_5(self):
        self.assertEqual(countdown(7, "fire"), "7. 6. 5. 4. 3. 2. 1. FIRE!")

    def test_6(self):
        self.assertEqual(
            countdown(16, "shoot"),
            "16. 15. 14. 13. 12. 11. 10. 9. 8. 7. 6. 5. 4. 3. 2. 1. SHOOT!",
        )

    def test_7(self):
        self.assertEqual(
            countdown(28, "fire"),
            "28. 27. 26. 25. 24. 23. 22. 21. 20. 19. 18. 17. 16. 15. 14. 13. 12. 11. 10. 9. 8. 7. 6. 5. 4. 3. 2. 1. FIRE!",
        )

    def test_8(self):
        self.assertEqual(
            countdown(14, "watch out"),
            "14. 13. 12. 11. 10. 9. 8. 7. 6. 5. 4. 3. 2. 1. WATCH OUT!",
        )

    def test_9(self):
        self.assertEqual(
            countdown(29, "take down"),
            "29. 28. 27. 26. 25. 24. 23. 22. 21. 20. 19. 18. 17. 16. 15. 14. 13. 12. 11. 10. 9. 8. 7. 6. 5. 4. 3. 2. 1. TAKE DOWN!",
        )

    def test_10(self):
        self.assertEqual(countdown(8, "boom"), "8. 7. 6. 5. 4. 3. 2. 1. BOOM!")


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Making a Countdown](https://edabit.com/challenge/7QvH8PJgQ5x4qNGLh)
