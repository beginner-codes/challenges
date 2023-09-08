# Challenge 746 - Microwave Buttons

In microwave ovens, when buttons are pressed from 0-9, it will add that number to the microwave oven timer (starting from the left). All microwave ovens have the functionality where you can hit a `"+30"` button and it will add 30 seconds to the timer to cook your food. If you want to heat something for 5 mins, you can hit the `"+30"` button 10 times instead of thinking if there are fewer button presses that can give you the same result.

Create a function that takes an argument time and returns the shortest amount of button presses to set the given time on the microwave oven. The microwave oven timer always starts at `00:00`.
```
Buttons
Buttons from "0-9"

# It will add that number to the microwave oven timer (starting from the left).
# If the number "5" is pressed followed by "0" twice, it will put 05:00 on the timer.
# If the number "3" is pressed followed by "0", it will put 00:30 on the timer.

Button "+30", which adds 30 seconds to the current timer.

# If the number "+30" is pressed twice, it will put 00:60 on the timer.

A "Start" button which you have to finally press to start the microwave oven.

# Remember to press this!
```
## Examples
```python
microwave_buttons("00:30") ➞ 2
# "+30" to put 30 seconds on the timer.
# "Start" button to start the oven.

microwave_buttons("00:70") ➞ 3
# "7" followed by "0" to put 70 seconds on the timer.
# "Start" button to start the oven.

microwave_buttons("00:00") ➞ 1
# "Start" button to start the oven.
```
## Notes

- Input may not always be what you expect (e.g. you can put in 00:70, which is valid).

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. *
*[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a
key `args` that are a list of parameters your function should take. The `return` key is what your function should return
given the `args`.

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your
solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:

```python
from __future__ import annotations
from beginnercodes.challenges import test


def microwave_buttons(time: str) -> int:
    return 0  # Put your code here!!!


test(746, microwave_buttons)  # Tell it which challenge to test against
```

And here's the JSON.

```json
[
    {
        "args": [
            "10:00"
        ],
        "return": 5
    },
    {
        "args": [
            "00:00"
        ],
        "return": 1
    },
    {
        "args": [
            "01:00"
        ],
        "return": 3
    },
    {
        "args": [
            "00:60"
        ],
        "return": 3
    },
    {
        "args": [
            "00:10"
        ],
        "return": 3
    }
]
```

## Credits

Found on Edabit: [Microwave Buttons](https://edabit.com/challenge/yXipH35Xv4cBa8pnm)
