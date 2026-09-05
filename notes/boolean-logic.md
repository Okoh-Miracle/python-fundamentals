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

## Operator Precedence

Python does not evaluate `and` and `or` from left to right equally.

`and` has higher precedence than `or`, so Python evaluates the `and` expression first.

For example:

```python
A or B and C
is evaluated as:
A or (B and C)
not:
(A or B) and C
Parentheses can be used when a different order is intended:
(A or B) and C
Precedence to remember

From higher to lower precedence:

not
and
or

When an expression becomes difficult to read, using parentheses can make the intended logic much clearer.

## Practical Example

Suppose:

```python
A = True
B = False
C = True

Consider:

A or B and C

Because and has higher precedence than or, Python evaluates:

B and C

first.

Since False and True is False, the expression becomes:

True or False

which evaluates to:

True

This is why understanding precedence matters when translating logic into Python.

## Common Mistakes

### 1. Assuming `and` and `or` have equal precedence

Python evaluates `and` before `or`.

```python
A or B and C

means:

A or (B and C)
2. Forgetting parentheses

If the intended logic is different from Python's default precedence, use parentheses explicitly.

(A or B) and C
3. Translating English logic too quickly

Statements such as "A or B and C" can be ambiguous in natural language. Writing the logic step by step and checking it with a truth table can help prevent mistakes.

## Related Concepts
Boolean values: True and False
Conditional statements
Comparison operators
Truth tables
Logical expressions
Operator precedence


