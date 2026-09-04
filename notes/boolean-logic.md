# Boolean Logic and Operator Precedence in Python

## Summary

Boolean logic allows a program to make decisions based on conditions that evaluate to `True` or `False`.

In Python, the main Boolean operators are `and`, `or`, and `not`. Understanding how these operators work — especially their precedence — is important because the order in which Python evaluates an expression can change its result.

## Key Boolean Operators

| Operator | Meaning |
|---|---|
| `and` | `True` when both conditions are `True` |
| `or` | `True` when at least one condition is `True` |
| `not` | Reverses a Boolean value |

Examples:

```python
True and True    # True
True and False   # False
True or False    # True
not True         # False
