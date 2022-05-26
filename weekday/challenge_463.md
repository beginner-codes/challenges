# Challenge 463 - Case and Index Inverter

Write a function that takes a string input and returns the string in a reversed case and order.

## Examples
```python
invert("dLROW YM sI HsEt") ➞ "TeSh iS my worlD"

invert("ytInIUgAsnOc") ➞ "CoNSaGuiNiTY"

invert("step on NO PETS") ➞ "step on NO PETS"

invert("XeLPMoC YTiReTXeD") ➞ "dExtErIty cOmplEx"
```
## Join Us & Share Your Solution

We're a community of coders who believe the best way to grow is to help others learn. **[Join us on Discord!!!]("https"://discord.gg/sfHykntuGy)**

## Challenge Tests

Here are a series of tests in JSON format that you can use to test your code. Each object in the JSON array has a key `args` that are a list of parameters your function should take. The `return` key is what your function should return given the `args`. 

If you're writing your solution in Python you can also use the `beginner.codes` Python package to automate testing your solution. Install it with `pip install beginner.codes`, then create a file for your solution and use the following code:
```python
from beginnercodes.challenges import test


def invert(string: str) -> str:
    return ""  # Put your code here!!!


test(463, invert)  # Tell it which challenge to test against
```
And here's the JSON.
```json
[
    {
        "args": [
            "dLROW YM sI HsEt"
        ],
        "return": "TeSh iS my worlD"
    },
    {
        "args": [
            "This string is CASE and INDEX reversed"
        ],
        "return": "DESREVER xedni DNA esac SI GNIRTS SIHt"
    },
    {
        "args": [
            "ReVeRsIbLe"
        ],
        "return": "ElBiSrEvEr"
    },
    {
        "args": [
            "rAmIfIcAtIoN"
        ],
        "return": "nOiTaCiFiMaR"
    },
    {
        "args": [
            "IntellectualS"
        ],
        "return": "sLAUTCELLETNi"
    },
    {
        "args": [
            "DESREVER xedni DNA esac SI GNIRTS SIHt"
        ],
        "return": "This string is CASE and INDEX reversed"
    },
    {
        "args": [
            "ElBiSrEvEr"
        ],
        "return": "ReVeRsIbLe"
    },
    {
        "args": [
            "nOiTaCiFiMaR"
        ],
        "return": "rAmIfIcAtIoN"
    },
    {
        "args": [
            "sLAUTCELLETNi"
        ],
        "return": "IntellectualS"
    },
    {
        "args": [
            "CoNSaGuiNiTY"
        ],
        "return": "ytInIUgAsnOc"
    },
    {
        "args": [
            "step on NO PETS"
        ],
        "return": "step on NO PETS"
    },
    {
        "args": [
            "dExtErIty cOmplEx"
        ],
        "return": "XeLPMoC YTiReTXeD"
    }
]
```
## Credits

Found on Edabit: [Case and Index Inverter](https://edabit.com/challenge/jyqcRv6giw8an8KB2)
