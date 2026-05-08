# 📘 Module 07: Arrays + Strings (Combined Logic)

---

## Learning Outcomes Assessed

* Array Processing
* String Manipulation
* Combined Data Logic
* Iterative Problem Solving
* Pattern Recognition
* Real-World Text Analysis

---

## Module Structure

This module contains:

### Coding Practice:

All questions must be completed inside:

```java id="m8x4pr"
ArrayStringExercises.java
```

Your task is to:

* Read each function carefully
* Understand how arrays and strings interact
* Break larger problems into smaller logical steps
* Process data safely using loops
* Handle formatting and validation carefully
* Return exact required outputs
* Pass all tests successfully

---

## Your Goal

For each function:

* Use valid Java syntax
* Combine arrays and strings effectively
* Handle substring and indexing safely
* Prevent boundary and logic errors
* Handle edge cases carefully
* Follow exact expected outputs
* Ensure all unit tests pass

---

## How to Run Your Tests

### Run all tests:

```bash id="d3q9lt"
mvn test
```

### Run module tests:

```bash id="k6n2vx"
mvn test -Dtest=ArrayStringExercisesTest
```

---

# 🧠 Core Combined Concepts

---

## Why Combine Arrays + Strings?

Real-world software often requires:

* Splitting text into parts
* Searching through collections of words
* Counting patterns in user input
* Processing structured text data
* Analyzing sequences step-by-step

---

## Common Skills Used

### String Iteration:

```java id="y5m8cu"
for (int i = 0; i < text.length(); i++) {
    char c = text.charAt(i);
}
```

---

### Array Traversal:

```java id="r9v3ke"
for (String word : arr) {
    // process each word
}
```

---

## Important Reminder

When combining strings and arrays:

* Check boundaries carefully
* Avoid index errors
* Use substring safely
* Validate lengths before processing
* Normalize case when needed

---

# 🧪 Fundamentals Coding Practice

---

## Project Structure

```plaintext id="t2w7bn"
module07/
├── ArrayStringExercises.java
├── tests/
│   └── ArrayStringExercisesTest.java
└── README.md
```

---

# Question 1 - splitString

## Function:

```java id="f7z2qm"
exercise1_splitString(String s, int length)
```

### Detailed Objective:

Create a method that splits a string into smaller chunks of a specified size.

This exercise teaches:

* Substring extraction
* Array creation
* Controlled string segmentation
* Handling uneven lengths

Your method should divide the original string into sections of the provided length.

If the final section has fewer characters than the requested size, it must still be included.

---

### Rules:

* Split string into chunks of `length`
* Preserve all characters
* Include smaller final chunk if necessary
* Return results as `String[]`

---

### Input:

* String `s`
* Integer `length`

---

### Output:

* Array of string chunks

---

### Examples:

| Input            | Output                      |
| ---------------- | --------------------------- |
| "hello world", 3 | ["hel", "lo ", "wor", "ld"] |
| "abcdefg", 2     | ["ab", "cd", "ef", "g"]     |
| "short", 10      | ["short"]                   |

---

### Edge Cases:

* Chunk size larger than string
* Exact division
* Empty strings
* Length of 1
* Invalid boundaries

---

# Question 2 - findLongestWord

## Function:

```java id="v4p8xn"
exercise2_findLongestWord(String[] arr)
```

### Detailed Objective:

Create a method that scans an array of words and returns the longest valid word.

This exercise teaches:

* Array scanning
* Conditional comparisons
* Ignoring invalid entries
* Tracking best matches

---

### Rules:

* Ignore empty strings
* Return the longest word
* If multiple words tie, return the first one

---

### Input:

* String array

---

### Output:

* Longest word

---

### Examples:

| Input                      | Output     |
| -------------------------- | ---------- |
| ["cat", "elephant", "dog"] | "elephant" |
| ["", "hello", "world"]     | "hello"    |
| ["one", "two", "six"]      | "one"      |

---

### Edge Cases:

* Empty strings
* All equal lengths
* Single-element arrays
* Multiple longest matches

---

# Question 3 - countVowels

## Function:

```java id="u1q7zk"
exercise3_countVowels(String s)
```

### Detailed Objective:

Create a method that counts how many times each vowel appears in a string.

This exercise teaches:

* Character-by-character processing
* Pattern counting
* Frequency arrays
* Case normalization

Your method must count occurrences of:

* `a`
* `e`
* `i`
* `o`
* `u`

---

### Return Format:

```java id="w6k3pv"
[aCount, eCount, iCount, oCount, uCount]
```

---

### Rules:

* Ignore non-letter characters
* Ignore consonants
* Count vowels only
* Case-insensitive if required by tests

---

### Input:

* String `s`

---

### Output:

* Integer array

---

### Examples:

| Input         | Output      |
| ------------- | ----------- |
| "hello world" | [0,1,0,2,0] |
| "aeiou"       | [1,1,1,1,1] |
| "bcdfg"       | [0,0,0,0,0] |

---

### Edge Cases:

* Empty strings
* Uppercase vowels
* No vowels
* Only vowels
* Symbols and spaces

---

# 💡 Key Developer Tips

* Always validate substring ranges
* Prevent out-of-bounds errors
* Normalize case for consistency
* Use loops carefully
* Track variables clearly
* Think step-by-step
* Handle unusual input safely

---

# 🚀 End Goal

By completing this module, you should:

* Combine multiple programming concepts effectively
* Process structured text confidently
* Solve layered logic problems
* Improve real-world coding ability
* Strengthen algorithmic thinking
* Build stronger debugging habits

---

# 🏆 Success Mindset

Professional software rarely uses isolated concepts.

Real development combines strings, arrays, loops, and logic simultaneously.

Mastering combined problem-solving is a major step toward becoming a stronger developer.
