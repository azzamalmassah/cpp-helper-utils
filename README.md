

# clsUtil – C++ Utility Helper Library

`clsUtil` is a header-only C++ utility class that provides a collection of commonly used helper functions for small to medium console projects. It’s designed mainly for **learning, practice, and reuse** while building C++ fundamentals like functions, references, arrays, strings, and basic algorithms.

This library groups many everyday tasks into one place: math helpers, random generators, array utilities, string utilities, and number-to-text conversion.

---

## ✨ Features

* 🔁 Multiple `Swap` overloads (int, double, bool, char, string)
* 🎲 Random utilities:

  * Random numbers in range
  * Random characters (capital, small, digit, special)
  * Random words
  * Random license-key style strings
* 📦 Array utilities:

  * Shuffle arrays
  * Fill arrays with random numbers, words, or keys
  * Search for number in array
  * Simple dynamic insert (manual size tracking)
* 🧮 Math helpers:

  * Average calculation
  * `Round`, `Floor`, `Ceil`, `Sqrt`, `Abs`
  * Reverse number
  * Digit frequency counter
* 🔐 String utilities:

  * Simple encryption / decryption (Caesar shift)
* 🔢 Convert numbers to English text (`NumberToText`)
* 🧪 Input helpers:

  * Read number in range
  * Validate age in range

---

## 🛠 Requirements

* C++11 or later
* Standard headers:

  * `<iostream>`
  * `<string>`
  * `<ctime>`
  * `<cstdlib>`
  * `<cmath>`

---

## 📦 Installation

Just include the header file in your project:

```
#include "clsUtil.h"
```

Make sure the file is in your include path.

---

## 🚀 Usage Examples

### Initialize Random Generator

Call this once at program start:

```
clsUtil::Srand();
```

---

### Generate a Random Key

```
std::string key = clsUtil::GenerateKey();
std::cout << key << std::endl;
```

Example output:

```
ABCD-QWER-ZXCV-ASDF
```

---

### Swap Two Values

```
int a = 5, b = 10;
clsUtil::Swap(a, b);
```

---

### Reverse a Number

```
int r = clsUtil::Reverse(12345); // 54321
```

---

### Encrypt / Decrypt Text

```
std::string encrypted = clsUtil::EncryptText("Hello", 2);
std::string decrypted = clsUtil::DecryptText(encrypted, 2);
```

---

### Shuffle an Array

```
int arr[100] = {1,2,3,4,5};
int len = 5;

clsUtil::ShuffleArray(arr, len);
```

---

### Convert Number to Text

```
std::cout << clsUtil::NumberToText(12345);
```

Output:

```
Twelve Thousands Three Hundreds Forty Five
```

---

## ⚠️ Notes & Limitations

* Arrays are fixed-size (`[100]`) and use manual length tracking.
* Some functions mix **logic and console I/O** (not ideal for large or testable projects).
* This library is intended for **learning and small projects**, not production use.
* Error handling is minimal by design (educational focus).

---

## 🧠 Learning Goals

This project demonstrates practice with:

* Static utility classes
* Function overloading and references
* Arrays and strings
* Random number generation
* Basic algorithms
* Recursion (`NumberToText`)
* Structuring reusable helper code

---

## 📄 License

Free to use for learning and personal projects.

---

If you want, I can tailor this README to your **GitHub profile**, add **badges**, or rewrite it to look more **portfolio / recruiter-friendly** 😎
