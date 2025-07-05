# ✅ TDD String Calculator in Java | Incubyte Assignment

This project is an implementation of the **String Calculator Kata** using **Test-Driven Development (TDD)** in Java, as part of the **Incubyte Campus Placement First Round Assignment**.

---

## 👨‍💻 Objective

To build a simple `StringCalculator` class in a **test-first** (TDD) manner that progressively supports parsing and summing numbers from strings, handling different delimiters, negative number checks, and tracking internal behavior — while always writing tests before code.

---

## 📌 Key Features (Based on Incubyte Requirements)

| #  | Requirement Summary                                                                 | ✅ Status |
|----|--------------------------------------------------------------------------------------|----------|
| 1  | Add method that handles empty, one, or two numbers                                   | ✅ Done   |
| 2  | Return 0 for empty string                                                            | ✅ Done   |
| 3  | Allow unknown number of inputs                                                       | ✅ Done   |
| 4  | Support newlines (`\n`) between numbers                                              | ✅ Done   |
| 5  | Support custom delimiter: `"//[delimiter]\n[numbers]"`                               | ✅ Done   |
| 6  | Throw exception for negative numbers                                                 | ✅ Done   |
| 7  | Show **all** negative numbers in exception                                           | ✅ Done   |
| 8  | Add `GetCalledCount()` method to return how many times `Add()` was called           | ✅ Done   |
| 9  | Ignore numbers greater than 1000                                                     | ✅ Done   |
| 10 | Support multi-character delimiters like `[***]`                                      | ✅ Done   |
| 11 | Allow multiple custom single-character delimiters like `[;][*]`                      | ✅ Done   |
| 12 | Allow multiple custom **multi-character** delimiters like `[**][%%]`                 | ✅ Done   |

---

## 🚀 Examples

```java
""                      => 0
"1"                     => 1
"1,2"                   => 3
"1\n2,3"                => 6
"//;\n1;2"              => 3
"//[***]\n1***2***3"    => 6
"//[*][%]\n1*2%3"       => 6
"//[**][%%]\n1**2%%3"   => 6
"2,1001"                => 2
"//;\n1;-2"             => Exception: negatives not allowed: [-2]
"//;\n-1;-2;3"          => Exception: negatives not allowed: [-1, -2]
