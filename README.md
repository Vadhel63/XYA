# 🧪 TDD-Based String Calculator | Incubyte Campus Placement Assignment

This project is a **TDD-first implementation** of the classic **String Calculator Kata**, submitted as part of the **Incubyte Campus Placement (Round 1)** assignment.

It demonstrates strict adherence to **Test-Driven Development**, clean Java practices, and comprehensive JUnit testing.

---

## 📌 What is TDD?

> **TDD (Test-Driven Development)** is a software development process where tests are written **before the actual code**. It follows the cycle:


📜 TDD Approach Followed

This assignment was developed using Test-Driven Development (TDD) strictly:

Wrote failing tests first (empty input, negative numbers, custom delimiters, etc.)

Wrote minimal code to make them pass.

Refactored after each test to keep the code clean and modular.

✔️ TDD Laws (by Uncle Bob):

You cannot write production code unless there is a failing test.

You cannot write more of a test than is sufficient to fail.

You cannot write more production code than is sufficient to pass the test.


In this project:
- I **started with the simplest tests** (empty string, single number)
- Gradually **added features** (custom delimiters, error handling, call count tracking)
- Always wrote **tests first**, then implementation
- Ensured all tests **stay green** throughout development

📚 Reference: [Three Laws of TDD by Uncle Bob](https://blog.cleancoder.com/uncle-bob/2014/12/17/TheCyclesOfTDD.html)

---
## ✅ Features Implemented

| #  | Requirement                                                                         | Status |
|----|-------------------------------------------------------------------------------------|--------|
| 1  |Return `0` for empty string                                                           | ✅ Done |
| 2  | Add method to sum 0, 1, or 2 numbers (`""`, `"1"`, `"1,2"`)                          | ✅ Done |
| 3  | Support unknown number of inputs (`"1,2,3,4"`)                                       | ✅ Done |
| 4  | Support newline as delimiter (`"1\n2,3"`)                                            | ✅ Done |
| 5  | Support custom single delimiter (`"//;\n1;2"`)                                       | ✅ Done |
| 6  | Throw exception for Single negative number (`"1,-2"` → `-2 not allowed`)             | ✅ Done |
| 7  | Throw exception for Multiple negative numbers (`"1,-2,-4"` → `-2,-4 not allowed`)    | ✅ Done |
| 8 | Show **all** negative numbers in exception message                                    | ✅ Done |
| 9  | Add `GetCalledCount()` method to track `Add()` calls                                  | ✅ Done |
| 10  | Ignore numbers greater than 1000 (`"2,1001"` → returns 2)                             | ✅ Done |
| 11 | Support multi-character delimiters like `[***]`                                       | ✅ Done |
| 12 | Support multiple single-char delimiters like `[;][*]`                                 | ✅ Done |
| 13 | Support multiple multi-char delimiters like `[**][%%]`                                | ✅ Done |

---

## 🧪 All Tests Passed ✅

Here’s a screenshot showing all my tests successfully passing:

> 🖼️ **Insert your screenshot below this line**  
> *(e.g., IntelliJ JUnit test results or terminal `mvn test` results)*

![All Tests Passing](screenshots/all-tests-pass.png)

---

## 💡 Sample Inputs & Outputs

| Input String                          | Expected Output / Behavior                |
|--------------------------------------|-------------------------------------------|
| `""`                                 | `0`                                       |
| `"7"`                                | `7`                                       |
| `"1,2"`                              | `3`                                       |
|`"1,3,6,2"`                           | `12`                                      | 
| `"1\n2,3"`                           | `6`                                       |
| `"//;\n1;2"`                         | `3`                                       |
|`"1,-2"`                              | Exception: `negative not allowed: -2`     |
|`"1,-2,-4"`                           | Exception: `negative not allowed: -2,-4`  |
| `"2,1001"`                           | `2`                                       |
| `"//[***]\n1***2***3"`               | `6`                                       |
| `"//[*][%]\n1*2%3"`                  | `6`                                       |
| `"//[**][%%]\n1**2%%3"`              | `6`                                       |


---

## 📂 Project Structure

TDD-Assesment_Incubyte/
├── src/
│ ├── main/java/org/VadhelMilan/StringCalculator.java
│ └── test/java/org/VadhelMilan/StringCalculatorTest.java
├── screenshots/
│ └── all-tests-pass.png ← Upload your test screenshot here
├── pom.xml
└── README.md

---

🧱 Technology Stack

☕ Java 8+

✅ JUnit 4.13.2

🧰 Maven (build tool)

📏 Regex (Pattern, Matcher) for delimiter parsing

---


## 🛠️ How to Run

1. Ensure Java 8+ and Maven are installed.
2. Clone the repository.
3. Run all tests with:

```bash
mvn clean test

---


---

## 🙏 Thank You

Thank you **Incubyte** for this opportunity.  
This assignment helped me sharpen my skills in **TDD**, **clean code**, and **unit testing**.  
I genuinely enjoyed learning and applying **Test-Driven Development** throughout this project.


With gratitude,  
**👨‍💻 Milan Vadhel**  

