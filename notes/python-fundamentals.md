# Python Fundamentals — Course Notes

These notes summarize the core concepts I have learned while working through Georgia Tech's CS1301xI: Computing in Python I.

## 1. Boolean Logic

Boolean values represent two possible states:

```python
True
False
```

### Comparison Operators

```text
>   greater than
<   less than
>=  greater than or equal to
<=  less than or equal to
==  equal to
!=  not equal to
```

Important:

```python
=   # assignment
==  # comparison
```

### Logical Operators

```python
and
or
not
```

Python's Boolean operator precedence is:

1. Parentheses
2. `not`
3. `and`
4. `or`

Example:

```python
A or B and C
```

is evaluated as:

```python
A or (B and C)
```

not:

```python
(A or B) and C
```

---

## 2. Arithmetic Operators

Python supports several arithmetic operations:

```python
+    addition
-    subtraction
*    multiplication
/    division
//   floor division
%    remainder
**   exponentiation
```

Example:

```python
10 / 3
10 // 3
10 % 3
10 ** 2
```

A useful pattern is quotient and remainder:

```python
quotient = total // size
remainder = total % size
```

---

## 3. Variables and Assignment

Variables store values.

```python
name = "Miracle"
age = 25
```

Assignment gives a variable a value at that moment. Changing another variable later does not create a permanent connection between the two values.

Compound assignment operators include:

```python
+=
-=
*=
/=
%=
**=
//=
```

Example:

```python
score = 10
score += 5
```

After this, `score` is `15`.

---

## 4. Types and Type Conversion

Common Python types include:

```python
int
float
str
bool
```

Python provides conversion functions:

```python
str()
int()
float()
bool()
```

Example:

```python
age = int("25")
price = float("19.99")
```

---

## 5. Strings

Strings represent text.

```python
name = "Miracle"
```

Strings can be combined with `+`:

```python
first = "Hello"
second = "World"

message = first + " " + second
```

Strings can also be repeated:

```python
"Hi " * 3
```

The `in` operator can check whether one string occurs inside another:

```python
"Python" in "I am learning Python"
```

---

## 6. Input and Output

`print()` displays information:

```python
print("Hello, world!")
```

`input()` allows a program to receive user input:

```python
name = input("What is your name? ")
```

Input is returned as a string, so conversion may be necessary when working with numbers:

```python
age = int(input("Enter your age: "))
```

---

## 7. Conditional Logic

`if` statements allow programs to make decisions.

```python
if age >= 18:
    print("Adult")
```

Conditions can be combined using Boolean operators:

```python
if age >= 18 and has_id:
    print("Allowed")
```

---

## 8. Mathematical Formulas

Python can be used to translate mathematical formulas into executable programs.

The `math` module provides mathematical constants and functions.

For example:

```python
import math

amount = principal * math.e ** (rate * time)
```

Python uses `**` for exponentiation.

Important:

```python
**   # exponentiation
^    # not exponentiation in Python
```

---

## 9. Floating-Point Numbers

Decimal calculations use floating-point numbers.

Because computers represent many decimal values approximately, calculations involving floating-point numbers can sometimes produce very small rounding differences.

Python provides `round()` when rounded output is needed:

```python
round(3.14159, 2)
```

---

## 10. Dates and Time

When solving date and time problems, it is important to identify the units being used.

For time calculations, converting everything into one unit can make the problem easier.

For example:

```text
hours → minutes
minutes → seconds
```

For dates, comparisons may require checking:

1. Year
2. Month
3. Day

---

## 11. Problem-Solving Patterns

A useful approach to programming problems is:

1. Read the rules carefully.
2. Identify the variables.
3. Translate each rule into a separate expression.
4. Combine the expressions.
5. Test the program using the current values.
6. Consider what happens when the values change.

Pay attention to wording such as:

* "at least" → `>=`
* "more than" → `>`
* "on or after" → `>=`
* "after" → `>`
* "unless" → carefully translate the exception into Boolean logic

---

## 12. Common Python Errors

### SyntaxError

The code does not follow Python's syntax rules.

### TypeError

An operation is being performed on an inappropriate type.

### NameError

Python cannot find the variable or name being referenced.

### ZeroDivisionError

A calculation attempts to divide by zero.

Understanding error messages is part of debugging.
