# 📘 Module 12: Exception Handling & File I/O

---

## Learning Outcomes Assessed

* Exception Handling
* Defensive Programming
* Try-Catch Logic
* Runtime Error Prevention
* File Writing
* File Reading
* File Processing
* Resource Management
* Java I/O
* Robust Software Development

---

## Module Structure

This module contains:

### Coding Practice:

Complete all functions inside:

```java
FileExercises.java
```

---

## Your Task

For this module, you must:

* Safely handle runtime errors
* Prevent program crashes
* Work with external files
* Read and write file data
* Manage invalid input
* Return exact outputs
* Use proper Java exception handling
* Pass all tests successfully

---

## Your Goal

For each function:

* Use valid Java syntax
* Use `try-catch` correctly
* Handle failures gracefully
* Prevent crashes
* Work with files safely
* Follow exact return requirements
* Ensure all unit tests pass

---

## How to Run Your Tests

### Run all tests:

```bash
mvn test
```

### Run module tests:

```bash
mvn test -Dtest=FileExercisesTest
```

---

# 🧠 Core Java Reliability Concepts

---

# 🔹 What Are Exceptions?

Exceptions are runtime errors that interrupt normal program execution.

---

### Common Examples:

* Division by zero
* Invalid number conversion
* Missing files
* Permission errors

---

### Without handling:

Your program crashes.

---

### With handling:

Your program safely recovers.

---

# 🔹 Why Exception Handling Matters

Professional software must:

* Avoid crashes
* Recover from bad input
* Handle missing resources
* Protect user experience
* Log failures safely

---

### Real-World Examples:

* User enters invalid number
* Server file missing
* Customer uploads corrupted data
* API receives malformed request

---

# 🔹 try-catch Structure

```java
try {
    // risky code
} catch (Exception e) {
    // fallback behavior
}
```

---

### Purpose:

Allows code to continue safely.

---

# 🔹 File I/O

File Input/Output allows programs to:

* Save user data
* Read configurations
* Process logs
* Store reports
* Persist information

---

# 🧪 Project Structure

```plaintext
module12/
├── FileExercises.java
├── tests/
│   └── FileExercisesTest.java
└── README.md
```

---

# Question 1 - Safe Division

## Function:

```java
exercise1_safeDivide(int a, int b)
```

---

### # 📘 Module 12: Exception Handling & File I/O

---

## Learning Outcomes Assessed

* Exception Handling

* Defensive Programming

* Try-Catch Logic

* Runtime Error Prevention

* File Writing

* File Reading

* File Processing

* Resource Management

* Java I/O

* Robust Software Development

---

## Module Structure

This module contains:

### Coding Practice:

Complete all functions inside:

```java id="v4m8qx"

FileExercises.java

```

---

## Your Task

For this module, you must:

* Safely handle runtime errors

* Prevent program crashes

* Work with external files

* Read and write file data

* Manage invalid input

* Return exact outputs

* Use proper Java exception handling

* Pass all tests successfully

---

## Your Goal

For each function:

* Use valid Java syntax

* Use `try-catch` correctly

* Handle failures gracefully

* Prevent crashes

* Work with files safely

* Follow exact return requirements

* Ensure all unit tests pass

---

## How to Run Your Tests

### Run all tests:

```bash id="n8v3pk"

mvn test

```

### Run module tests:

```bash id="x2m7qt"

mvn test -Dtest=FileExercisesTest

```

---

# 🧠 Core Java Reliability Concepts

---

# 🔹 What Are Exceptions?

Exceptions are runtime errors that interrupt normal program execution.

---

### Common Examples:

* Division by zero

* Invalid number conversion

* Missing files

* Permission errors

---

### Without handling:

Your program crashes.

---

### With handling:

Your program safely recovers.

---

# 🔹 Why Exception Handling Matters

Professional software must:

* Avoid crashes

* Recover from bad input

* Handle missing resources

* Protect user experience

* Log failures safely

---

### Real-World Examples:

* User enters invalid number

* Server file missing

* Customer uploads corrupted data

* API receives malformed request

---

# 🔹 try-catch Structure

```java id="k7v4mx"

try {

    // risky code

} catch (Exception e) {

    // fallback behavior

}

```

---

### Purpose:

Allows code to continue safely.

---

# 🔹 File I/O

File Input/Output allows programs to:

* Save user data

* Read configurations

* Process logs

* Store reports

* Persist information

---

# 🧪 Project Structure

```plaintext id="p3m8qw"

module12/

├── FileExercises.java

├── tests/

│   └── FileExercisesTest.java

└── README.md

```

---

# Question 1 - Safe Division

## Function:

```java id="r5v7pk"

exercise1_safeDivide(int a, int b)

```

---

### Detailed Objective:

Create a division method that prevents crashes when dividing by zero.

---

### Rules:

* Return `a / b`

* If `b == 0` → return `0`

---

### Examples:

| Input   | Output |

| ------- | ------ |

| (10, 2) | 5      |

| (9, 3)  | 3      |

| (5, 0)  | 0      |

---

### Why This Matters:

Division by zero is a common runtime error.

Your method must protect against this.

---

### Developer Skill Built:

* Arithmetic safety

* Exception prevention

* Defensive coding

---

# Question 2 - Parse Integer Safely

## Function:

```java id="t9m4xv"

exercise2_parseInteger(String value)

```

---

### Detailed Objective:

Convert text into an integer safely.

---

### Rules:

* Valid integer → return parsed value

* Invalid input → return `-1`

---

### Examples:

| Input | Output |

| ----- | ------ |

| "123" | 123    |

| "-45" | -45    |

| "abc" | -1     |

| ""    | -1     |

---

### Real-World Context:

User forms often contain invalid input.

Your program must recover safely.

---

### Developer Skill Built:

* Input validation

* Parsing safety

* Error recovery

---

# Question 3 - Write File

## Function:

```java id="f8v2qr"

exercise3_writeFile(String fileName, String content)

```

---

### Detailed Objective:

Write text content into a file.

---

### Rules:

* Write provided content

* Return `true` if successful

* Return `false` if failure occurs

---

### Examples:

| Input                  | Output |

| ---------------------- | ------ |

| ("notes.txt", "Hello") | true   |

| Invalid path           | false  |

---

### Real-World Uses:

* Saving reports

* Config files

* User settings

* Logs

---

### Important:

Always close file resources properly.

---

# Question 4 - Read File

## Function:

```java id="j3m9qx"

exercise4_readFile(String fileName)

# 📘 Module 12: Exception Handling & File I/O

---

## Learning Outcomes Assessed

* Exception Handling

* Defensive Programming

* Try-Catch Logic

* Runtime Error Prevention

* File Writing

* File Reading

* File Processing

* Resource Management

* Java I/O

* Robust Software Development

---

## Module Structure

This module contains:

### Coding Practice:

Complete all functions inside:

```java id="v4m8qx"

FileExercises.java

```

---

## Your Task

For this module, you must:

* Safely handle runtime errors

* Prevent program crashes

* Work with external files

* Read and write file data

* Manage invalid input

* Return exact outputs

* Use proper Java exception handling

* Pass all tests successfully

---

## Your Goal

For each function:

* Use valid Java syntax

* Use `try-catch` correctly

* Handle failures gracefully

* Prevent crashes

* Work with files safely

* Follow exact return requirements

* Ensure all unit tests pass

---

## How to Run Your Tests

### Run all tests:

```bash id="n8v3pk"

mvn test

```

### Run module tests:

```bash id="x2m7qt"

mvn test -Dtest=FileExercisesTest

```

---

# 🧠 Core Java Reliability Concepts

---

# 🔹 What Are Exceptions?

Exceptions are runtime errors that interrupt normal program execution.

---

### Common Examples:

* Division by zero

* Invalid number conversion

* Missing files

* Permission errors

---

### Without handling:

Your program crashes.

---

### With handling:

Your program safely recovers.

---

# 🔹 Why Exception Handling Matters

Professional software must:

* Avoid crashes

* Recover from bad input

* Handle missing resources

* Protect user experience

* Log failures safely

---

### Real-World Examples:

* User enters invalid number

* Server file missing

* Customer uploads corrupted data

* API receives malformed request

---

# 🔹 try-catch Structure

```java id="k7v4mx"

try {

    // risky code

} catch (Exception e) {

    // fallback behavior

}

```

---

### Purpose:

Allows code to continue safely.

---

# 🔹 File I/O

File Input/Output allows programs to:

* Save user data

* Read configurations

* Process logs

* Store reports

* Persist information

---

# 🧪 Project Structure

```plaintext id="p3m8qw"

module12/

├── FileExercises.java

├── tests/

│   └── FileExercisesTest.java

└── README.md

```

---

# Question 1 - Safe Division

## Function:

```java id="r5v7pk"

exercise1_safeDivide(int a, int b)

```

---

### Detailed Objective:

Create a division method that prevents crashes when dividing by zero.

---

### Rules:

* Return `a / b`

* If `b == 0` → return `0`

---

### Examples:

| Input   | Output |

| ------- | ------ |

| (10, 2) | 5      |

| (9, 3)  | 3      |

| (5, 0)  | 0      |

---

### Why This Matters:

Division by zero is a common runtime error.

Your method must protect against this.

---

### Developer Skill Built:

* Arithmetic safety

* Exception prevention

* Defensive coding

---

# Question 2 - Parse Integer Safely

## Function:

```java id="t9m4xv"

exercise2_parseInteger(String value)

```

---

### Detailed Objective:

Convert text into an integer safely.

---

### Rules:

* Valid integer → return parsed value

* Invalid input → return `-1`

---

### Examples:

| Input | Output |

| ----- | ------ |

| "123" | 123    |

| "-45" | -45    |

| "abc" | -1     |

| ""    | -1     |

---

### Real-World Context:

User forms often contain invalid input.

Your program must recover safely.

---

### Developer Skill Built:

* Input validation

* Parsing safety

* Error recovery

---

# Question 3 - Write File

## Function:

```java id="f8v2qr"

exercise3_writeFile(String fileName, String content)

```

---

### Detailed Objective:

Write text content into a file.

---

### Rules:

* Write provided content

* Return `true` if successful

* Return `false` if failure occurs

---

### Examples:

| Input                  | Output |

| ---------------------- | ------ |

| ("notes.txt", "Hello") | true   |

| Invalid path           | false  |

---

### Real-World Uses:

* Saving reports

* Config files

* User settings

* Logs

---

### Important:

Always close file resources properly.

---

# Question 4 - Read File

## Function:

```java id="j3m9qx"

exercise4_readFile(String fileName)

```

---

### Detailed Objective:

Read all file content safely.

---

### Rules:

* Return full file content

* If error → return empty string `""`

---

### Examples:

| File Content | Output        |

| ------------ | ------------- |

| Hello World  | "Hello World" |

| Missing file | ""            |

---

### Real-World Uses:

# 📘 Module 12: Exception Handling & File I/O

---

## Learning Outcomes Assessed

* Exception Handling
* Defensive Programming
* Try-Catch Logic
* Runtime Error Prevention
* File Writing
* File Reading
* File Processing
* Resource Management
* Java I/O
* Robust Software Development

---

## Module Structure

This module contains:

### Coding Practice:

Complete all functions inside:

```java id="v4m8qx"
FileExercises.java
```

---

## Your Task

For this module, you must:

* Safely handle runtime errors
* Prevent program crashes
* Work with external files
* Read and write file data
* Manage invalid input
* Return exact outputs
* Use proper Java exception handling
* Pass all tests successfully

---

## Your Goal

For each function:

* Use valid Java syntax
* Use `try-catch` correctly
* Handle failures gracefully
* Prevent crashes
* Work with files safely
* Follow exact return requirements
* Ensure all unit tests pass

---

## How to Run Your Tests

### Run all tests:

```bash id="n8v3pk"
mvn test
```

### Run module tests:

```bash id="x2m7qt"
mvn test -Dtest=FileExercisesTest
```

---

# 🧠 Core Java Reliability Concepts

---

# 🔹 What Are Exceptions?

Exceptions are runtime errors that interrupt normal program execution.

---

### Common Examples:

* Division by zero
* Invalid number conversion
* Missing files
* Permission errors

---

### Without handling:

Your program crashes.

---

### With handling:

Your program safely recovers.

---

# 🔹 Why Exception Handling Matters

Professional software must:

* Avoid crashes
* Recover from bad input
* Handle missing resources
* Protect user experience
* Log failures safely

---

### Real-World Examples:

* User enters invalid number
* Server file missing
* Customer uploads corrupted data
* API receives malformed request

---

# 🔹 try-catch Structure

```java id="k7v4mx"
try {
    // risky code
} catch (Exception e) {
    // fallback behavior
}
```

---

### Purpose:

Allows code to continue safely.

---

# 🔹 File I/O

File Input/Output allows programs to:

* Save user data
* Read configurations
* Process logs
* Store reports
* Persist information

---

# 🧪 Project Structure

```plaintext id="p3m8qw"
module12/
├── FileExercises.java
├── tests/
│   └── FileExercisesTest.java
└── README.md
```

---

# Question 1 - Safe Division

## Function:

```java id="r5v7pk"
exercise1_safeDivide(int a, int b)
```

---

### Detailed Objective:

Create a division method that prevents crashes when d* Loading saved settings

* Reading logs

* Processing documents

---

### Developer Skill Built:

* File reading

* Error handling

* Resource safety

---

# Question 5 - Count File Lines

## Function:

```java id="m7v4zt"

exercise5_countLines(String fileName)

```

---

### Detailed Objective:

Count total lines in a file.

---

### Rules:

* Return line count

* If file missing/error → return `0`

---

### Examples:

| File         | Output |

| ------------ | ------ |

| 3-line file  | 3      |

| Empty file   | 0      |

| Missing file | 0      |

---

### Real-World Applications:

* Log analysis

* CSV processing

* Data validation

* File audits

---

### Developer Skill Built:

* Sequential file reading

* Counting logic

* Robust processing

---

# 💡 Key Developer Tips

* Always expect failure

* Never trust user input

* Use `try-catch` carefully

* Prefer `try-with-resources`

* Close files automatically

* Handle invalid paths

* Protect against crashes

* Build resilient software

---

# 🔹 Professional Mindset

Strong developers do not only write working code.

They write code that survives bad input, missing resources, and unexpected failures.

---

### Weak Code:

Crashes easily.

### Strong Code:

Handles errors professionally.

---

# 🚀 End Goal

By completing this module, you should:

* Understand Java exceptions deeply

* Handle runtime failures confidently

* Parse data safely

* Read files correctly

* Write files securely

* Build fault-tolerant applications

* Improve production readiness

* Write professional-grade Java programs

---

# 🏆 Success Mindset

Exception handling and file I/O are essential for:

* Enterprise applications

* Backend development

* APIs

* Automation

* Data engineering

* Software reliability

Mastering this module moves you closer to real-world software engineering, where stability matters as much as functionality.

```

---

### Detailed Objective:

Read all file content safely.

---

### Rules:

* Return full file content

* If error → return empty string `""`

---

### Examples:

| File Content | Output        |

| ------------ | ------------- |

| Hello World  | "Hello World" |

| Missing file | ""            |

---

### Real-World Uses:

* Loading saved settings

* Reading logs

* Processing documents

---

### Developer Skill Built:

* File reading

* Error handling

* Resource safety

---

# Question 5 - Count File Lines

## Function:

```java id="m7v4zt"

exercise5_countLines(String fileName)

```

---

### Detailed Objective:

Count total lines in a file.

---

### Rules:

* Return line count

* If file missing/error → return `0`

---

### Examples:

| File         | Output |

| ------------ | ------ |

| 3-line file  | 3      |

| Empty file   | 0      |

| Missing file | 0      |

---

### Real-World Applications:

* Log analysis

* CSV processing

* Data validation

* File audits

---

### Developer Skill Built:

* Sequential file reading

* Counting logic

* Robust processing

---

# 💡 Key Developer Tips

* Always expect failure

* Never trust user input

* Use `try-catch` carefully

* Prefer `try-with-resources`

* Close files automatically

* Handle invalid paths

* Protect against crashes

* Build resilient software

---

# 🔹 Professional Mindset

Strong developers do not only write working code.

They write code that survives bad input, missing resources, and unexpected failures.

---

### Weak Code:

Crashes easily.

### Strong Code:

Handles errors professionally.

---

# 🚀 End Goal

By completing this module, you should:

* Understand Java exceptions deeply

* Handle runtime failures confidently

* Parse data safely

* Read files correctly

* Write files securely

* Build fault-tolerant applications

* Improve production readiness

* Write professional-grade Java programs

---

# 🏆 Success Mindset

Exception handling and file I/O are essential for:

* Enterprise applications

* Backend development

* APIs

* Automation

* Data engineering

* Software reliability

Mastering this module moves you closer to real-world software engineering, where stability matters as much as functionality.

Detailed Objective:

Create a division method that prevents crashes when dividing by zero.

---

### Rules:

* Return `a / b`
* If `b == 0` → return `0`

---

### Examples:

| Input   | Output |
| ------- | ------ |
| (10, 2) | 5      |
| (9, 3)  | 3      |
| (5, 0)  | 0      |

---

### Why This Matters:

Division by zero is a common runtime error.

Your method must protect against this.

---

### Developer Skill Built:

* Arithmetic safety
* Exception prevention
* Defensive coding

---

# Question 2 - Parse Integer Safely

## Function:

```java
exercise2_parseInteger(String value)
```

---

### Detailed Objective:

Convert text into an integer safely.

---

### Rules:

* Valid integer → return parsed value
* Invalid input → return `-1`

---

### Examples:

| Input | Output |
| ----- | ------ |
| "123" | 123    |
| "-45" | -45    |
| "abc" | -1     |
| ""    | -1     |

---

### Real-World Context:

User forms often contain invalid input.

Your program must recover safely.

---

### Developer Skill Built:

* Input validation
* Parsing safety
* Error recovery

---

# Question 3 - Write File

## Function:

```java
exercise3_writeFile(String fileName, String content)
```

---

### Detailed Objective:

Write text content into a file.

---

### Rules:

* Write provided content
* Return `true` if successful
* Return `false` if failure occurs

---

### Examples:

| Input                  | Output |
| ---------------------- | ------ |
| ("notes.txt", "Hello") | true   |
| Invalid path           | false  |

---

### Real-World Uses:

* Saving reports
* Config files
* User settings
* Logs

---

### Important:

Always close file resources properly.

---

# Question 4 - Read File

## Function:

```java
exercise4_readFile(String fileName)
```

---

### Detailed Objective:

Read all file content safely.

---

### Rules:

* Return full file content
* If error → return empty string `""`

---

### Examples:

| File Content | Output        |
| ------------ | ------------- |
| Hello World  | "Hello World" |
| Missing file | ""            |

---

### Real-World Uses:

* Loading saved settings
* Reading logs
* Processing documents

---

### Developer Skill Built:

* File reading
* Error handling
* Resource safety

---

# Question 5 - Count File Lines

## Function:

```java
exercise5_countLines(String fileName)
```

---

### Detailed Objective:

Count total lines in a file.

---

### Rules:

* Return line count
* If file missing/error → return `0`

---

### Examples:

| File         | Output |
| ------------ | ------ |
| 3-line file  | 3      |
| Empty file   | 0      |
| Missing file | 0      |

---

### Real-World Applications:

* Log analysis
* CSV processing
* Data validation
* File audits

---

### Developer Skill Built:

* Sequential file reading
* Counting logic
* Robust processing

---

# 💡 Key Developer Tips

* Always expect failure
* Never trust user input
* Use `try-catch` carefully
* Prefer `try-with-resources`
* Close files automatically
* Handle invalid paths
* Protect against crashes
* Build resilient software

---

# 🔹 Professional Mindset

Strong developers do not only write working code.

They write code that survives bad input, missing resources, and unexpected failures.

---

### Weak Code:

Crashes easily.

### Strong Code:

Handles errors professionally.

---

# 🚀 End Goal

By completing this module, you should:

* Understand Java exceptions deeply
* Handle runtime failures confidently
* Parse data safely
* Read files correctly
* Write files securely
* Build fault-tolerant applications
* Improve production readiness
* Write professional-grade Java programs

---

# 🏆 Success Mindset

Exception handling and file I/O are essential for:

* Enterprise applications
* Backend development
* APIs
* Automation
* Data engineering
* Software reliability

Mastering this module moves you closer to real-world software engineering, where stability matters as much as functionality.
