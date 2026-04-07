# Palindrome-Mathematical-Python
A simple Python program that takes user input and checks if the reverse of that string equal to the original (Palindrome) Mathematically.
# 🔢 Palindrome Number Checker

## 📌 Description

This Python program checks whether a given integer is a **palindrome** or not.
A palindrome number is a number that reads the same **forward and backward** (e.g., 121, 1331).

---

## ⚙️ How It Works

* Negative numbers are **not palindrome**.
* Numbers ending with `0` (except `0` itself) are **not palindrome**.
* The program reverses the number using a loop.
* Finally, it compares the reversed number with the original.

---

## 🧠 Algorithm

1. Store the original number.
2. Reverse the number using modulo (`%`) and division (`//`).
3. Compare the reversed number with the original.
4. Return `True` if equal, otherwise `False`.

---

## 💻 Code Example

```python
class Solution(object):
    def isPalindrome(self, x):
        if x < 0 or (x % 10 == 0 and x != 0):
            return False

        original = x
        rev = 0

        while x > 0:
            rev = rev * 10 + x % 10
            x //= 10

        return original == rev


x = 9
obj = Solution()
print(obj.isPalindrome(x))
```

---

## ▶️ Sample Output

```
True
```

---

## 📥 Input

* An integer value (e.g., `9`, `121`, `123`)

## 📤 Output

* `True` → if the number is a palindrome
* `False` → if the number is not a palindrome

---

## 🚀 Features

* Simple and efficient logic
* No string conversion used
* Works for all integer inputs

---

## 📚 Example Cases

| Input | Output |
| ----- | ------ |
| 121   | True   |
| 123   | False  |
| -121  | False  |
| 10    | False  |

---

## 🛠️ Requirements

* Python 3.x

---

## 📄 License

Free to use for learning and educational purposes.
