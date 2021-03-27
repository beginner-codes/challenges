# Challenge 212 - Maze Escape

Given a maze as a two-dimensional list and a list of directions, create a function that follows the directions through the maze.

- If you can reach the endpoint before all your moves have gone, return `"Finish"`.
- If you hit any walls or go outside the maze border, return `"Dead"`.
- If you find yourself still in the maze after using all the moves, return `"Lost"`.

The maze list will look like this:
```python
maze = [
[1, 1, 1, 1, 1, 1, 1, 1, 0, 1],
[1, 3, 1, 0, 1, 0, 0, 0, 0, 1],
[1, 0, 1, 0, 0, 0, 1, 1, 0, 1],
[1, 0, 1, 1, 1, 1, 1, 0, 0, 1],
[1, 0, 1, 0, 0, 0, 0, 0, 0, 1],
[1, 0, 1, 0, 1, 0, 1, 0, 0, 1],
[1, 0, 1, 0, 1, 0, 0, 0, 0, 0],
[1, 0, 1, 0, 1, 0, 1, 1, 0, 1],
[1, 0, 0, 0, 1, 0, 0, 0, 0, 1],
[1, 1, 1, 0, 1, 1, 1, 1, 2, 1]
]
```
`0` = Safe place to walk  
`1` = Wall  
`2` = Start Point  
`3` = Finish Point  
`N` = North, `E` = East, `W` = West and `S` = South

## Examples
```python
exit_maze(maze, ["N", "E", "E"]) ➞ "Dead"
# Hitting the wall should return "Dead".
exit_maze(maze, ["N", "N", "N", "E"]) ➞ "Lost"
# Couldn't reach the finish point.
exit_maze(maze, ["N", "W", "W", "W", "N", "N", "N", "N", "W", "W", "S", "S", "S", "S", "W", "W", "N", "N", "N", "N", "N", "N", "N"]) ➞ "Finish"
```

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests
```python
from __future__ import annotations
import unittest


Maze = list[list[int]]
Directions = list[str]


def exit_maze(maze: Maze, directions: Directions) -> str:
    return ""  # Put your code here!!!


class Tests(unittest.TestCase):
    maze = [
        [1, 1, 1, 1, 1, 1, 1, 1, 0, 1],
        [1, 3, 1, 0, 1, 0, 0, 0, 0, 1],
        [1, 0, 1, 0, 0, 0, 1, 1, 0, 1],
        [1, 0, 1, 1, 1, 1, 1, 0, 0, 1],
        [1, 0, 1, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 1, 0, 1, 0, 1, 0, 0, 1],
        [1, 0, 1, 0, 1, 0, 0, 0, 0, 0],
        [1, 0, 1, 0, 1, 0, 1, 1, 0, 1],
        [1, 0, 0, 0, 1, 0, 0, 0, 0, 1],
        [1, 1, 1, 0, 1, 1, 1, 1, 2, 1],
    ]

    def test_1(self):
        self.assertEquals(
            exit_maze(
                self.maze,
                ["N", "N", "N", "W", "W", "W", "N", "N", "W", "W", "S", "S", "S", "S", "W", "W", "N", "N", "N", "N", "N", "N", "N"],
            ),
            "Finish",
        )

    def test_2(self):
        self.assertEquals(
            exit_maze(
                self.maze,
                ["N", "N", "N", "N", "N", "N", "N", "N", "W", "W", "W", "S", "W", "W", "N"],
            ),
            "Lost",
        )

    def test_3(self):
        self.assertEquals(
            exit_maze(
                self.maze,
                ["N","N", "N", "N", "N", "E", "E", "S", "S", "S", "S", "S", "S"],
            ),
            "Dead",
        )

    def test_4(self):
        self.assertEquals(exit_maze(self.maze, ["N","W", "W", "W", "W"]), "Dead")

    def test_5(self):
        self.assertEquals(
            exit_maze(
                self.maze,
                ["N", "N", "N", "N", "N", "N", "N", "N", "N", "S", "S", "S", "S", "S", "S", "S", "S", "S"],
            ),
            "Lost",
        )

    def test_6(self):
        self.assertEquals(exit_maze(self.maze, ["N","E",  "E"]), "Dead")

    def test_7(self):
        self.assertEquals(
            exit_maze(
                self.maze,
                ["N", "W", "W", "W", "N", "N", "N", "N", "W", "W", "S", "S", "S", "S", "W", "W", "N", "N", "N", "N", "N", "N", "N", "S", "S"],
            ),
            "Finish",
        )

    def test_8(self):
        self.assertEquals(exit_maze(self.maze, ["N","W", "W", "W", "N", "N"]), "Lost")

    def test_9(self):
        self.assertEquals(exit_maze(self.maze, ["N","N", "N", "E"]), "Lost")

    def test_10(self):
        self.assertEquals(
            exit_maze(
                self.maze,
                ["N", "N", "N", "W", "W", "W", "N", "N", "W", "W", "S", "S", "S", "S", "S", "S"],
            ),
            "Dead",
        )

    def test_11(self):
        self.assertEquals(
            exit_maze(
                self.maze,
                ["N", "W", "W", "W", "N", "N", "N", "N", "W", "W", "S", "S", "S", "S", "W", "W", "N", "N", "N", "N", "N", "N", "N"],
            ),
            "Finish",
        )


if __name__ == "__main__":
    unittest.main()
```
## Credits

Found on Edabit: [Maze Escape](https://edabit.com/challenge/tbz5ji3ocwzAeLQNa)
