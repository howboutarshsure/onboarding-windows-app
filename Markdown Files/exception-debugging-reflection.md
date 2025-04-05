# 🧩 Exception Handling & Debugging Reflection – C#

## 🎯 Task Overview

I created a small C# program that deliberately triggers a `DivideByZeroException`. I wrapped the risky operation in a `try-catch-finally` block to handle the error gracefully and used Visual Studio's debugging tools to step through the code and observe the flow during an exception.

---

## 🔍 Research & Learn

### ✅ Best Practices for Exception Handling in C#

- **Catch only what you can handle**: Avoid catching `Exception` unless necessary.
- **Use specific exception types**: Like `IOException`, `FormatException`, `DivideByZeroException`, etc.
- **Log exceptions**: Always log exception details for diagnostics.
- **Avoid swallowing exceptions silently**: At least log or rethrow them.
- **Use `finally`**: For cleanup tasks (e.g., closing files, releasing resources).
- **Don’t use exceptions for control flow**: Use validation logic instead.

### ✅ How try-catch-finally Works

- `try` block contains code that may throw exceptions
- `catch` block handles specific or general exceptions
- `finally` block always runs, whether an exception occurred or not

```csharp
try
{
    int result = 10 / 0;
}
catch (DivideByZeroException ex)
{
    Console.WriteLine("You can't divide by zero.");
}
finally
{
    Console.WriteLine("This always executes.");
}
```

### ✅ Debugging Tools in Visual Studio

- **Breakpoints**: Pause execution to inspect code
- **Locals & Watch Windows**: View current values of variables
- **Call Stack**: Shows the current execution path
- **Immediate Window**: Run expressions during debugging
- **Exception Settings**: Set Visual Studio to break on specific exceptions
- **Output Window**: Monitor runtime messages and logs

---

## 📝 Reflection

### ✅ When Exception Handling Prevented an Issue

In a past WPF project, I had a file reader method that occasionally failed due to missing files. Wrapping the logic in a `try-catch` block prevented the entire application from crashing and allowed me to show a user-friendly message instead.

### ✅ Most Effective Debugging Techniques

- **Step Into (F11)** to trace execution line-by-line
- **Breakpoints** to pause before risky operations
- **Watch Window** to track variable changes
- **Exception Settings** to break exactly where an exception is thrown

### ✅ Improving Error Logging & Reporting

- Use a logging framework like **Serilog** or **NLog**
- Log stack traces and error context
- Display clear but non-technical messages to users
- Send logs to a central location (e.g., file, database, or cloud service)

---

## ✅ Summary

Proper exception handling and debugging are essential to developing robust applications. Using `try-catch-finally` blocks prevents crashes and improves the user experience. Visual Studio’s built-in debugging tools made it easy to observe and understand exception behavior, helping me become more efficient in identifying and fixing issues.
