# 📘 Module 08: Varargs & Enhanced Switch

---

## Learning Outcomes Assessed

* Varargs (`...`)
* Enhanced Switch Expressions
* Flexible Method Design
* Multi-Input Processing
* Modern Java Syntax
* Structured Decision Logic

---

## Module Structure

This module contains:

### Coding Practice:

All questions must be completed inside:

```java id="p8v4tm"
VarargsSwitchExercises.java
```

Your task is to:

* Read each function carefully
* Understand flexible parameter handling
* Apply enhanced switch expressions properly
* Process multiple inputs efficiently
* Return exact required outputs
* Handle edge cases carefully
* Pass all tests successfully

---

## Your Goal

For each function:

* Use valid Java syntax
* Implement varargs correctly
* Use enhanced switch expressions
* Avoid unnecessary if/else structures where prohibited
* Handle empty or invalid inputs safely
* Follow exact return formats
* Ensure all unit tests pass

---

## How to Run Your Tests

### Run all tests:

```bash id="w3k7rq"
mvn test
```

### Run module tests:

```bash id="h9x2cv"
mvn test -Dtest=VarargsSwitchExercisesTest
```

---

# 🧠 Core Modern Java Concepts

---

## What is Varargs?

Varargs (`...`) allows methods to accept a variable number of arguments.

---

### Example:

```java id="q4m8zn"
public static int sum(int... numbers)
```

---

### Why Varargs Matter

Varargs allows:

* Flexible input sizes
* Cleaner APIs
* Easier method calls
* Reduced overload complexity

---

### Important Reminder:

Internally, varargs behaves like an array.

---

## What is Enhanced Switch?

Enhanced switch expressions provide:

* Cleaner syntax
* Improved readability
* Safer control flow
* Direct return values

---

### Example:

```java id="j2v9pk"
String result = switch(day) {
    case "MONDAY", "TUESDAY" -> "Weekday";
    default -> "Invalid";
};
```

---

# 🧪 Fundamentals Coding Practice

---

## Project Structure

```plaintext id="u5d3mx"
module08/
├── VarargsSwitchExercises.java
├── tests/
│   └── VarargsSwitchExercisesTest.java
└── README.md
```

---

# Question 1 - Sum Numbers (Varargs)

## Function:

```java id="g8x4lp"
exercise1_sumNumbers(int... numbers)
```

### Detailed Objective:

Create a method that accepts any number of integers and returns their total sum.

This exercise teaches:

* Varargs processing
* Dynamic input handling
* Looping through flexible argument lists

---

### Rules:

* Add all numbers together
* If no numbers are provided, return:

```java id="n7q3wd"
0
```

---

### Input:

* Variable number of integers

---

### Output:

* Integer sum

---

### Examples:

| Input       | Output |
| ----------- | ------ |
| (1, 2, 3)   | 6      |
| (10, -5, 2) | 7      |
| ()          | 0      |

---

### Edge Cases:

* Empty input
* Negative values
* Large lists
* Zero values

---

# Question 2 - Find Max (Varargs)

## Function:

```java id="k4z7tv"
exercise2_findMax(int... numbers)
```

### Detailed Objective:

Create a method that returns the largest number from a flexible list of integers.

---

### Rules:

* Return maximum value
* If no numbers are provided:

```java id="v1m8yc"
Integer.MIN_VALUE
```

---

### Input:

* Variable number of integers

---

### Output:

* Maximum integer

---

### Examples:

| Input        | Output            |
| ------------ | ----------------- |
| (5, 2, 9)    | 9                 |
| (-1, -5, -2) | -1                |
| ()           | Integer.MIN_VALUE |

---

### Edge Cases:

* Empty input
* Negative-only inputs
* Single value

---

# Question 3 - Count Even Numbers (Varargs)

## Function:

```java id="t9w2qx"
exercise3_countEven(int... numbers)
```

### Detailed Objective:

Create a method that counts how many provided numbers are even.

---

### Rules:

* Count values divisible by 2
* Return total even count

---

### Input:

* Variable number of integers

---

### Output:

* Integer count

---

### Examples:

| Input        | Output |
| ------------ | ------ |
| (1, 2, 3, 4) | 2      |
| (2, 4, 6)    | 3      |
| (1, 3, 5)    | 0      |

---

### Edge Cases:

* Empty input
* Zero
* Negative evens

---

# Question 4 - Day Type (Enhanced Switch)

## Function:

```java id="m3q7bz"
exercise4_dayType(String day)
```

### Detailed Objective:

Determine whether a provided day is a weekday or weekend.

This exercise focuses on:

* Enhanced switch syntax
* Grouped conditions
* Text-based decision making

---

### Rules:

* MONDAY–FRIDAY → `"Weekday"`
* SATURDAY–SUNDAY → `"Weekend"`
* Anything else → `"Invalid day"`

---

### Input:

* Day string

---

### Output:

* Classification string

---

### Examples:

| Input      | Output        |
| ---------- | ------------- |
| "MONDAY"   | "Weekday"     |
| "SATURDAY" | "Weekend"     |
| "HOLIDAY"  | "Invalid day" |

---

### Edge Cases:

* Invalid spelling
* Case sensitivity
* Empty strings

---

# Question 5 - Grade Evaluator (Enhanced Switch)

## Function:

```java id="x7v5mp"
exercise5_gradeEvaluator(String grade)
```

### Detailed Objective:

Evaluate academic letter grades into performance descriptions.

---

### Rules:

* A → `"Excellent"`
* B → `"Good"`
* C → `"Average"`
* D → `"Poor"`
* F → `"Fail"`
* Default → `"Invalid grade"`

---

### Input:

* Grade string

---

### Output:

* Evaluation string

---

### Examples:

| Input | Output          |
| ----- | --------------- |
| "A"   | "Excellent"     |
| "C"   | "Average"       |
| "F"   | "Fail"          |
| "Z"   | "Invalid grade" |

---

### Edge Cases:

* Invalid grades
* Lowercase depending on tests
* Empty values

---

# Question 6 - Simple Calculator (Enhanced Switch)

## Function:

```java id="r5k9tx"
exercise6_calculator(double a, double b, String operator)
```

### Detailed Objective:

Create a calculator that performs basic arithmetic based on a provided operator.

---

### Supported Operators:

* `+`
* `-`
* `*`
* `/`

---

### Rules:

* Perform correct operation
* Division by zero → return `0`
* Invalid operator handling depends on tests

---

### Input:

* Double `a`
* Double `b`
* Operator string

---

### Output:

* Double result

---

### Examples:

| Input      | Output |
| ---------- | ------ |
| 5, 3, "+"  | 8      |
| 10, 2, "/" | 5      |
| 7, 0, "/"  | 0      |

---

### Edge Cases:

* Division by zero
* Invalid operators
* Negative numbers
* Decimal values

---

# Question 7 - Month Days (Enhanced Switch)

## Function:

```java id="y2n8qf"
exercise7_monthDays(String month)
```

### Detailed Objective:

Return the number of days in a given month.

---

### Rules:

* January → 31
* February → 28
* April → 30
* Invalid month → -1

---

### Input:

* Month string

---

### Output:

* Integer days

---

### Examples:

| Input      | Output |
| ---------- | ------ |
| "JANUARY"  | 31     |
| "FEBRUARY" | 28     |
| "APRIL"    | 30     |
| "INVALID"  | -1     |

---

### Edge Cases:

* Invalid month names
* Case sensitivity
* Empty strings

---

# 💡 Key Developer Tips

* Varargs behaves like arrays
* Always validate empty input
* Enhanced switch improves readability
* Group related cases efficiently
* Handle defaults properly
* Watch out for division by zero
* Test multiple scenarios carefully

---

# 🚀 End Goal

By completing this module, you should:

* Use varargs confidently
* Build flexible reusable methods
* Master enhanced switch syntax
* Process dynamic inputs efficiently
* Improve modern Java proficiency
* Strengthen scalable coding habits

---

# 🏆 Success Mindset

Modern Java emphasizes flexibility, clarity, and maintainability.

Mastering varargs and enhanced switch prepares you for cleaner enterprise-level development and more professional software design.
