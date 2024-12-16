## Challenge: Fibonacci
-# December 15th, 2024

For this challenge you must create a function that returns the Nth fibonacci number.

The fibonacci sequence is computed by adding the previous two numbers in the sequence to get the next number. The sequence begins with 1, the next number in the sequence is 1 (0 + 1), followed by 2 (1 + 1), then 3 (1 + 2), and so on.

To solve this challenge you must implement a function that takes an integer `nth`, generates the fibonacci numbers until it reaches the `nth` number in the sequence, and finally returns that number.

```py
fib(0) => 1
fib(1) => 1
fib(2) => 2
fib(3) => 3
fib(4) => 5
fib(10) => 89
```

Numbers in the sequence get very large very quickly with the 10,000th number being 2,090 digits long and only the 93rd exceeding the limits of a 64 bit unsigned int. So depending on the language chosen you might need to use some more advanced concepts to generate larger values.

## Test Cases

You can download test cases with this command:

```shell
curl https://raw.githubusercontent.com/beginner-codes/challenges/refs/heads/main/2024/12/15/test_cases.json > 20241215_test_cases.json
```

They're stored as JSON using this schema:

```json
[
  {
    "parameters": [10],
    "expected_result": "89"
  },
  ...
]
```

The expected result is always stringified to allow for results that may exceed the bounds of an integer.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**