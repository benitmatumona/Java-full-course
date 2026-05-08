# 📘 Module 03: Loops (`while`, `do-while`, `for`)

---

## Learning Outcomes Assessed

* Repetition Logic
* Loop Structures
* Flow Control
* Data Processing
* Break & Continue
* Iterative Problem Solving

---

## Module Structure

This module contains:

### Coding Practice:

All questions must be completed inside:

```java id="1kj1wa"
LoopExercises.java
```

Your task is to:

* Read each function carefully
* Determine which loop is most appropriate
* Apply correct looping logic
* Handle stopping conditions properly
* Return exact expected outputs
* Pass all tests successfully

---

## Your Goal

For each function:

* Use valid Java syntax
* Choose the correct loop (`while`, `do-while`, or `for`)
* Prevent infinite loops
* Handle edge cases carefully
* Follow formatting instructions precisely
* Ensure all unit tests pass

---

## How to Run Your Tests

### Run all tests:

```bash id="spj79n"
mvn test
```

### Run module tests:

```bash id="96j14g"
mvn test -Dtest=LoopExercisesTest
```

---

# 🧠 Core Loop Concepts

---

## `while` Loop

Used when the number of repetitions is unknown and continues while a condition remains true.

```java id="sj20vv"
while (condition) {
    // repeat
}
```

---

## `do-while` Loop

Executes at least once before checking the condition.

```java id="u1ujx5"
do {
    // executes first
} while (condition);
```

---

## `for` Loop

Best used when the number of repetitions is known.

```java id="53d24l"
for (int i = 0; i < limit; i++) {
    // repeat
}
```

---

## `break`

Stops the loop immediately when a condition is met.

---

## `continue`

Skips the current iteration and proceeds to the next.

---

# 🧪 Fundamentals Coding Practice

---

## Project Structure

```plaintext id="h71u2l"
module03/
├── LoopExercises.java
├── tests/
│   └── LoopExercisesTest.java
└── README.md
```

---

# Question 1 - Guessing Game

## Function:

```java id="6lcm2w"
exercise1_guessingGame(int[] guesses, int secret)
```

### Detailed Objective:

Simulate repeated guesses until the correct value is found.

### Rules:

* Count each guess attempt
* Stop once the secret is guessed
* Return total attempts

---

### Input:

* `int[] guesses`
* `int secret`

### Output:

* Integer number of attempts

---

### Examples:

| Input                 | Output |
| --------------------- | ------ |
| [5, 7], secret = 7    | 2      |
| [3, 4, 9], secret = 9 | 3      |
| [8], secret = 8       | 1      |

---

### Edge Cases:

* Secret guessed immediately
* Multiple failed attempts before success
* Secret always exists in array

---

# Question 2 - PIN Validator

## Function:

```java id="1j3s3e"
exercise2_pinValidator(int[] pins)
```

### Detailed Objective:

Validate repeated PIN attempts until the correct PIN (`1234`) is entered.

### Rules:

* Count each attempt
* Stop immediately when correct PIN is entered
* Return total attempts

---

### Input:

* `int[] pins`

### Output:

* Integer number of attempts

---

### Examples:

| Input              | Output |
| ------------------ | ------ |
| [1111, 1234]       | 2      |
| [1234]             | 1      |
| [0000, 9999, 1234] | 3      |

---

### Edge Cases:

* Correct PIN entered first
* Multiple failed attempts
* Assume correct PIN eventually appears

---

# Question 3 - Sum Until Zero

## Function:

```java id="1m5o9d"
exercise3_sumUntilZero(int[] numbers)
```

### Detailed Objective:

Continuously sum numbers until `0` appears.

### Rules:

* Add numbers in sequence
* Stop immediately when `0` is encountered
* Do not include `0` in the sum

---

### Input:

* `int[] numbers`

### Output:

* Integer sum

---

### Examples:

| Input        | Output |
| ------------ | ------ |
| [5, 3, 2, 0] | 10     |
| [1, 2, 3, 0] | 6      |
| [0]          | 0      |

---

### Edge Cases:

* Zero appears first
* Negative values may still be included before zero

---

# Question 4 - Number Printer

## Function:

```java id="4fwsxv"
exercise4_numberPrinter(int n)
```

### Detailed Objective:

Print numbers from `1` to `n`, skipping multiples of 5.

### Rules:

* Use a `for` loop
* Skip all numbers divisible by 5
* Return numbers as a comma-separated string

---

### Input:

* Integer `n`

### Output:

* Formatted string

---

### Examples:

| Input | Output                   |
| ----- | ------------------------ |
| 10    | "1, 2, 3, 4, 6, 7, 8, 9" |
| 5     | "1, 2, 3, 4"             |
| 3     | "1, 2, 3"                |

---

### Edge Cases:

* `n < 5`
* Exact multiples of 5
* Proper comma formatting

---

# Question 5 - Password Checker

## Function:

```java id="0ptl5m"
exercise5_passwordChecker(String[] attempts)
```

### Detailed Objective:

Allow a maximum of 3 password attempts to enter the correct password (`"secret"`).

### Rules:

* Maximum 3 attempts
* Stop early if password is correct
* Return:

```java id="h48lr8"
"Access granted!"
```

or

```java id="up6n4t"
"Access denied"
```

---

### Input:

* `String[] attempts`

### Output:

* Access result string

---

### Examples:

| Input                          | Output            |
| ------------------------------ | ----------------- |
| ["wrong", "secret"]            | "Access granted!" |
| ["wrong1", "wrong2", "wrong3"] | "Access denied"   |
| ["secret"]                     | "Access granted!" |

---

### Edge Cases:

* Correct password on first try
* More than 3 attempts provided
* No successful attempt

---

# Question 6 - Even Numbers

## Function:

```java id="7i4n0h"
exercise6_evenNumbers(int n)
```

### Detailed Objective:

Print all even numbers from `1` to `n`.

### Rules:

* Use `continue` to skip odd numbers
* Return even values as comma-separated string

---

### Input:

* Integer `n`

### Output:

* Formatted string

---

### Examples:

| Input | Output       |
| ----- | ------------ |
| 8     | "2, 4, 6, 8" |
| 5     | "2, 4"       |
| 2     | "2"          |

---

### Edge Cases:

* `n < 2`
* Large ranges
* Proper output formatting

---

# 💡 Key Developer Tips

* Always update counters properly
* Prevent infinite loops
* Watch for off-by-one mistakes
* Use `break` strategically
* Use `continue` carefully
* Test stopping conditions thoroughly
* Format strings precisely

---

# 🚀 End Goal

By completing this module, you should:

* Understand when to use each loop type
* Build strong repetition logic
* Control program flow effectively
* Solve iterative problems confidently
* Improve debugging and logic-building skills
* Prepare for advanced algorithms and data structures

---

# 🏆 Success Mindset

Loops are one of the most powerful tools in software engineering.

From automation systems to AI workflows to enterprise software, repetition drives efficient programming.

Master loops thoroughly before progressing.
