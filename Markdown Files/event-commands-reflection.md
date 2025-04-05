# ⚡ Event Handling & Commands Reflection – WPF

## 🎯 Task Overview

To explore the differences between standard event handling and WPF commands, I created a simple WPF application with a button that updates a label when clicked.

Initially, I handled the button click using a **standard event handler** in the code-behind. Later, I refactored the app to use a **command-based approach** through the `ICommand` interface in line with the **MVVM pattern**.

---

## 🔍 Research & Learn

### ✅ Routed Events vs Standard Events in WPF

- **Standard Events**: Work like regular .NET events (e.g., Button.Click += ...).
- **Routed Events**: Travel up or down the visual tree. WPF supports:
  - **Bubbling**: Event starts from the source and bubbles up (e.g., Button.Click).
  - **Tunneling**: Event starts from the root and tunnels down (`PreviewMouseDown`).
  - **Direct**: Handled like standard .NET events with no routing.

### ✅ What Are Commands in WPF?

Commands encapsulate actions and enable **separation of concerns**. Instead of handling events in the code-behind, you bind UI controls to command properties in ViewModels.

- Supports features like `CanExecute`, command reusability, and testability.
- Commonly used in MVVM architecture with `ICommand`.

### ✅ ICommand Interface

- `ICommand.Execute(object parameter)`: Defines the action to perform.
- `ICommand.CanExecute(object parameter)`: Determines if command can run.
- `CanExecuteChanged`: Raised when command execution ability changes.

---

## 📝 Reflection

### ✅ Maintainability Benefits of Commands

Using commands helps keep the UI logic out of the code-behind, making the app easier to test, debug, and maintain. It promotes cleaner code and encourages the use of **ViewModels** in MVVM design.

### ✅ When Commands Are Better

- When the same action is bound to multiple UI elements.
- When you want to disable/enable buttons dynamically (`CanExecute`).
- When following the MVVM pattern strictly without UI logic in the view.

### ✅ Challenges with Commands

- Slightly more boilerplate code (e.g., implementing `ICommand`).
- More complex for beginners unfamiliar with MVVM.
- Debugging command binding errors can be tricky without tools or Output window messages.

---

## ✅ Summary

Both event handling and commands have their place in WPF development. Standard events are quick and intuitive for small projects, while commands scale better in large, MVVM-based applications. By refactoring my button click example to use a command, I saw firsthand how it improved code structure and separation of concerns.

This understanding is crucial for building maintainable and testable WPF applications.
