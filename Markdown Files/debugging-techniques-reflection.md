# 🐞 Debugging Techniques Reflection – Visual Studio for WPF

## 🎯 Project Overview

For this task, I created a simple WPF application that accepts two numbers and performs a division operation. I deliberately introduced a bug by not checking for a zero denominator, which causes a `DivideByZeroException`.

Using Visual Studio's debugging tools, I was able to identify, inspect, and resolve the issue efficiently.

---

## 🔍 Research & Learn

### ✅ Key Debugging Features in Visual Studio

- **Breakpoints**: Pause execution at a specific line to inspect variables and flow.
- **Watch Window**: Monitor the values of selected variables during runtime.
- **Locals Window**: Automatically shows variables in the current scope.
- **Call Stack**: Shows the function call sequence leading to the current point.
- **Immediate Window**: Allows evaluating expressions or executing code while debugging.
- **Live Visual Tree & Live Property Explorer**: Inspect WPF UI elements in real-time.
- **Output Window**: Displays runtime logs, data binding errors, and system messages.

### ✅ Using These Tools to Inspect Runtime State

- Set breakpoints at critical lines (e.g., just before a calculation)
- Use Watch or Locals window to monitor values of variables step by step
- Use Immediate Window to change values or test quick expressions
- Use Live Visual Tree to trace UI element hierarchy and properties
- Observe the Output window to catch WPF-specific errors like data binding failures

### ✅ Best Practices for Debugging WPF Issues

- Enable `PresentationTraceSources.TraceLevel` for XAML bindings
- Use `Dispatcher.Invoke()` for UI thread access if modifying UI from background threads
- Use the Output window to catch binding errors (they won’t throw exceptions)
- Inspect DataContext and binding paths using Live Property Explorer
- Break large logic into smaller testable pieces to isolate bugs faster

---

## 📝 Reflection

### ✅ Most Useful Tools

I found **Breakpoints**, the **Output Window**, and the **Live Visual Tree** particularly helpful. Breakpoints let me pause and track variables step by step, while the Output Window helped me catch XAML binding errors that didn’t cause crashes.

### ✅ Debugging Scenario

In my WPF app, the TextBox input for the denominator was not validated. The user entered 0, which caused a crash. Setting a breakpoint and inspecting the variable helped me confirm the problem. I then added logic to prevent division by zero and show a warning message instead.

### ✅ Impact on Productivity

Improving my debugging skills has a big impact on productivity. Instead of guessing what went wrong, I now use a methodical approach. It reduces time spent on trial-and-error and helps ensure my fixes are correct the first time.

---

## ✅ Conclusion

Visual Studio provides powerful tools for debugging WPF applications. By using breakpoints, the Output Window, and the Live Visual Tree, I was able to trace and fix UI and logic issues efficiently. These skills are essential for maintaining high-quality, user-friendly WPF applications.
