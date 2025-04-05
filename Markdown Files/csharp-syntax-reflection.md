# 🧠 C# Syntax & Data Types Reflection

## 🎯 Task Summary

For this task, I wrote a simple C# program that demonstrates the use of `int`, `string`, and `bool` data types along with basic arithmetic and logical operators. I also experimented with type conversions, both implicit and explicit, to see how they behave in different scenarios.

---

## 🔍 Research & Learn

### ✅ Primary Data Types in C#

| Type     | Example       | Description                       |
|----------|---------------|-----------------------------------|
| `int`    | `int age = 25;` | Whole numbers                    |
| `string` | `string name = "Alex";` | Text data              |
| `bool`   | `bool isValid = true;` | True or false values   |
| `double` | `double pi = 3.14;` | Decimal numbers             |
| `char`   | `char grade = 'A';` | Single character             |
| `decimal`| `decimal price = 9.99m;` | High-precision decimal   |

### ✅ Variables, Constants, and Operators

- **Variables**: Mutable containers for data (e.g., `int count = 5;`)
- **Constants**: Immutable values (e.g., `const double Pi = 3.14;`)
- **Operators**:
  - Arithmetic: `+`, `-`, `*`, `/`, `%`
  - Logical: `&&`, `||`, `!`
  - Comparison: `==`, `!=`, `<`, `>`, `<=`, `>=`

### ✅ Type Conversion Pitfalls

- **Implicit conversion** is safe (e.g., `int` to `double`)
- **Explicit conversion** (casting) may lose data or cause exceptions
- `Convert.ToInt32()` vs `int.Parse()` — `Parse()` can throw if null or empty
- Boxing/unboxing can cause performance overhead

---

## 📝 Reflection

### ✅ Surprising Aspects

I found it interesting how strictly C# enforces type safety. For example, trying to assign a `double` to an `int` without casting causes a compile-time error, unlike some loosely typed languages.

### ✅ Data Types and Performance

- Choosing the right data type matters. For example, using `decimal` over `double` for financial calculations ensures accuracy but uses more memory.
- Overusing boxed types (like `object`) introduces performance penalties due to boxing/unboxing.

### ✅ Avoiding Type-Related Errors

- Always prefer `TryParse()` over `Parse()` for user input
- Be cautious with implicit casting between numeric types
- Use `var` for readability, but avoid overusing it where type clarity matters
- Avoid using `object` unless absolutely needed

---

## ✅ Summary

Understanding C# syntax and data types is fundamental to writing safe and efficient code. Practicing variable declaration, operators, and type conversions has helped me appreciate how strict type checking can prevent bugs and improve code clarity. This knowledge lays a strong foundation for further WPF and C# development.
