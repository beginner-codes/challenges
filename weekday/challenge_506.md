# Challenge 506 - CMS Selector Based on a Given String

Write a function that takes a list of strings and a pattern (string) and returns the strings that contain the pattern in alphabetical order. If the pattern is an empty string, return all the strings passed in the input list.

## Examples
```python
cms_selector(["WordPress", "Joomla", "Drupal"], "w") ➞ ["WordPress"]

cms_selector(["WordPress", "Joomla", "Drupal", "Magento"], "ru") ➞ ["Drupal"]

cms_selector(["WordPress", "Joomla", "Drupal", "Magento"], "") ➞ ["Drupal", "Joomla", "Magento", "WordPress"]
```
## Notes

- The given letter(s) are case insensitive and can be more than one.
- In the case of an empty string, return the entire list.
- A CMS is a Content Management System.

## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!](https://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from __future__ import annotations
from beginnercodes.challenges import test


def cms_selector(cms_list: list[str], search: str) -> list[str]:
    return []  # Put your code here!!!


test(506, cms_selector)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            [
                "WordPress",
                "Joomla",
                "Drupal",
                "Magento",
                "Shopify",
                "Blogger"
            ],
            "er"
        ],
        "return": [
            "Blogger"
        ]
    },
    {
        "args": [
            [
                "WordPress",
                "Joomla",
                "Drupal",
                "Magento",
                "Shopify",
                "Blogger"
            ],
            "o"
        ],
        "return": [
            "Blogger",
            "Joomla",
            "Magento",
            "Shopify",
            "WordPress"
        ]
    },
    {
        "args": [
            [
                "WordPress",
                "Joomla",
                "Drupal",
                "Magento",
                "Shopify",
                "Blogger"
            ],
            ""
        ],
        "return": [
            "Blogger",
            "Drupal",
            "Joomla",
            "Magento",
            "Shopify",
            "WordPress"
        ]
    },
    {
        "args": [
            [
                "WordPress",
                "Joomla",
                "Drupal",
                "Magento",
                "Shopify",
                "Blogger"
            ],
            "JO"
        ],
        "return": []
    }
]
```
## Credits

Found on Edabit: [CMS Selector Based on a Given String](https://edabit.com/challenge/whEretKtpEbEBAAfr)
