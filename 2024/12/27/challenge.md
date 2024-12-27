## Challenge: Well-Formed Parentheses
-# December 27th, 2024

For this challenge you must create a function that returns all "well-formed" combinations of `N` parentheses.

Given a value `N` generate all valid combinations of opening and closing parenthesis pairs where each closing parenthesis has a matching opening parenthesis before it in the output. 

So for `N` of 2 you'd output "()()" and "(())" as there are two pairs of opening and closing parentheses where the closing parenthesis always follows the opening one.

For `N` of 1 you'd output only "()". You'd not output ")(" because the opening parenthesis comes after it's closing pair. 

```py
parentheses(0) => []
parentheses(1) => ["()"]
parentheses(2) => ["(())", "()()"]
parentheses(3) => ["((()))", "(()())", "(())()", "()(())", "()()()"]
parentheses(4) => [
    "(((())))", 
    "((()()))",
    "((())())",
    "((()))()",
    "(()(()))",
    "(()()())",
    "(()())()",
    "(())(())",
    "(())()()",
    "()((()))",
    "()(()())",
    "()(())()",
    "()()(())",
    "()()()()"
]
```

## Test Cases

You can download test cases with this command:

```shell
curl https://raw.githubusercontent.com/beginner-codes/challenges/refs/heads/main/2024/12/27/test_cases.json > 20241227_test_cases.json
```

They're stored as JSON using this schema:

```json
[
  {
    "parameters": [2],
    "expected_result": ["()()", "(())"]  
  },
  ...
]
```

The results are always sorted in ascending ASCII order with duplicates removed.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**