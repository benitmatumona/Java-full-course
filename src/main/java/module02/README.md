# 📘 Module 02: Conditionals (`if / else`)

---

## Learning Outcomes Assessed

* Decision Making
* Conditional Logic
* Comparison Operators
* String Formatting
* Boundary Testing
* Problem Solving

---

## Module Structure

This module contains:

### Coding Practice:

All questions must be completed inside:

```java
ConditionExercises.java
```

Your task is to:

* Read each function carefully
* Understand what the function is asking
* Apply correct conditional logic
* Follow exact return formats
* Pass all tests successfully

---

## Your Goal

For each function:

* Use valid Java syntax
* Apply `if`, `else if`, and `else` correctly
* Handle all edge cases
* Return exact required outputs
* Follow formatting instructions precisely
* Ensure all unit tests pass

---

## How to Run Your Tests

### Run all tests:

```bash
mvn test
```

### Run module tests:

```bash
mvn test -Dtest=ConditionExercisesTest
```

---

# 🧠 Core Conditional Concepts

---

## `if` Statement

Used when code should only execute if a condition is true.

```java
if (condition) {
    // code runs
}
```

---

## `if / else`

Used when there are two possible outcomes.

```java
if (condition) {
    // true case
} else {
    // false case
}
```

---

## `if / else if / else`

Used when multiple conditions must be evaluated.

```java
if (condition1) {
    // first condition
} else if (condition2) {
    // second condition
} else {
    // default
}
```

---

## Comparison Operators

| Operator | Meaning               |
| -------- | --------------------- |
| `>`      | Greater than          |
| `<`      | Less than             |
| `>=`     | Greater than or equal |
| `<=`     | Less than or equal    |
| `==`     | Equal                 |
| `!=`     | Not equal             |

---

# 🧪 Fundamentals Coding Practice

---

## Project Structure

```plaintext
module02/
├── ConditionExercises.java
├── tests/
│   └── ConditionExercisesTest.java
└── README.md
```

---

# Question 1 - Temperature Alert

## Function:

```java
exercise1_temperatureAlert(int temperature)
```

### Detailed Objective:

Determine whether a temperature reading is considered hot.

### Rules:

* If temperature is above 30°C:

```java
"It's hot!"
```

* Otherwise:

```java
"It's not hot."
```

---

### Input:

* Integer temperature

### Output:

* String message

---

### Examples:

| Input | Output          |
| ----- | --------------- |
| 25    | "It's not hot." |
| 30    | "It's not hot." |
| 35    | "It's hot!"     |

---

### Edge Cases:

* Exactly 30 is NOT hot
* Negative temperatures are not hot

---

# Question 2 - Age Verification

## Function:

```java
exercise2_ageVerification(int age)
```

### Detailed Objective:

Verify whether a user meets the minimum age requirement.

### Rules:

* Age 18 or older:

```java
"Access granted"
```

* Otherwise:

```java
"Access denied"
```

---

### Input:

* Integer age

### Output:

* String access result

---

### Examples:

| Input | Output           |
| ----- | ---------------- |
| 17    | "Access denied"  |
| 18    | "Access granted" |
| 25    | "Access granted" |

---

### Edge Cases:

* Exactly 18 grants access
* Negative values deny access

---

# Question 3 - Even or Odd

## Function:

```java
exercise3_evenOrOdd(int number)
```

### Detailed Objective:

Determine whether a number is even or odd.

### Rules:

* Even:

```java
"X is even"
```

* Odd:

```java
"X is odd"
```

(`X` represents the actual number)

---

### Input:

* Integer number

### Output:

* Formatted string

---

### Examples:

| Input | Output      |
| ----- | ----------- |
| 4     | "4 is even" |
| 7     | "7 is odd"  |
| 0     | "0 is even" |

---

### Edge Cases:

* Zero is even
* Negative numbers can be even or odd

---

# Question 4 - Discount Calculator

## Function:

```java
exercise4_discountCalculator(double price)
```

### Detailed Objective:

Calculate discount percentage based on purchase amount.

### Rules:

* Above 1000 → 20%
* Between 500 and 1000 → 10%
* Below 500 → 0%

---

### Output Format:

```java
Discount: X%, Final price: RXXXX.XX
```

---

### Input:

* Double price

### Output:

* Formatted pricing string

---

### Examples:

| Input | Output                              |
| ----- | ----------------------------------- |
| 1200  | Discount: 20%, Final price: R960.00 |
| 750   | Discount: 10%, Final price: R675.00 |
| 300   | Discount: 0%, Final price: R300.00  |

---

### Edge Cases:

* 500 gets 10%
* 1000 gets 10%
* Correct currency formatting required

---

# Question 5 - Weather Advisor

## Function:

```java
exercise5_weatherAdvisor(int temperature)
```

### Detailed Objective:

Categorize weather conditions based on temperature.

### Rules:

* Above 30:

```java
"It's hot!"
```

* 15 to 30:

```java
"It's mild."
```

* Below 15:

```java
"It's cold."
```

---

### Input:

* Integer temperature

### Output:

* Weather description string

---

### Examples:

| Input | Output       |
| ----- | ------------ |
| 35    | "It's hot!"  |
| 20    | "It's mild." |
| 10    | "It's cold." |

---

### Edge Cases:

* 15 = mild
* 30 = mild

---

# Question 6 - Age Group

## Function:

```java
exercise6_ageGroup(int age)
```

### Detailed Objective:

Categorize individuals into age groups.

### Rules:

* Under 13:

```java
"Child"
```

* 13 to 19:

```java
"Teen"
```

* 20 and above:

```java
"Adult"
```

---

### Input:

* Integer age

### Output:

* Category string

---

### Examples:

| Input | Output  |
| ----- | ------- |
| 10    | "Child" |
| 15    | "Teen"  |
| 25    | "Adult" |

---

### Edge Cases:

* 13 = Teen
* 19 = Teen
* 20 = Adult

---

# 💡 Key Developer Tips

* Pay close attention to boundaries
* Be precise with comparison operators
* Follow exact output formatting
* Use `String.format()` when necessary
* Test all edge cases carefully

---

# 🚀 End Goal

By completing this module, you should:

* Build strong decision-making logic
* Understand branching conditions thoroughly
* Handle multiple outcomes confidently
* Improve debugging precision
* Strengthen real-world programming ability

---

# 🏆 Success Mindset

Conditional logic forms the backbone of intelligent software.

From security systems to weather apps to robotics, software constantly makes decisions.

Master conditionals thoroughly before progressing.
