# Java Exception Handling

This README provides brief answers to common questions about exception handling in Java.

## 1. How to Handle Exceptions in Java?

- Use try-catch blocks to encapsulate code that may throw exceptions.
- Catch specific exceptions or groups of exceptions to handle them appropriately.
- Optionally, include a finally block for cleanup operations.

## 2. Why is Exception Handling Important?

- Ensures graceful handling of errors, preventing crashes.
- Provides feedback to users about what went wrong.
- Helps maintain software stability and reliability.

## 3. Superclass for All Exceptions and Errors

- `java.lang.Throwable` serves as the superclass for both exceptions and errors.

## 4. Superclass for All Exceptions

- `java.lang.Exception` is the superclass for all exceptions, excluding errors.

## 5. Keywords for Exception Handling in Java

- Keywords include try, catch, finally, throw, and throws.

## 6. Different Types of Exceptions in Java

- Includes checked exceptions (Exception class and subclasses) and unchecked exceptions (RuntimeException and its subclasses).

## 7. Can Statements be Written Between try and catch Blocks?

- Yes, statements can be written between try and catch blocks.

## 8. Common Design Pattern for Exception Handling

- The Try-Catch pattern is commonly used for exception handling.

## 9. Purpose of finally Block

- The finally block ensures that certain code executes regardless of whether an exception occurred.

## 10. Scenarios Where Code in finally is Not Executed

- Code in finally may not execute if the JVM exits abruptly or if there's an infinite loop or System.exit() call within try or catch.

## 11. Is try Without a catch Allowed?

- Yes, try without catch is allowed if followed by finally or catch.

## 12. Definition of Exception Handler in Java

- An exception handler is a block of code responsible for catching and handling exceptions.

## 13. Code that Catches the Exception Thrown by JVM

- Typically found in the main method or methods at the top of the call stack.

## 14. Can try be Used Without finally and catch Blocks?

- No, try must be followed by finally or catch blocks.

## 15. Hierarchy of Exception Handling Classes

- Starts with Throwable, which has Error and Exception subclasses, with Exception further subclassing into checked and unchecked exceptions.

## 16. Difference between System.out.println(1/0) and System.out.println(2.0/0)

- First throws ArithmeticException, second prints Infinity due to floating-point behavior.

## 17. Difference between Error and Exception

- Errors are irrecoverable conditions, while exceptions represent errors in code or unexpected conditions.

## 18. Difference between Checked and Unchecked Exceptions

- Checked exceptions are checked at compile-time, while unchecked exceptions are not.

## 19. Exception Class to Handle Both Checked Exceptions

- java.lang.Exception can handle both checked exceptions.

## 20. Difference between throw and throws Keywords

- throw is used to raise an exception, while throws is used to declare exceptions that a method may throw.

## 21. How to Throw an Exception from a Method?

- Use the throw keyword followed by the exception object.

## 22. What Happens When a Checked Exception is Thrown from a Method?

- Must be caught using try-catch or declared using throws in the method signature.

## 23. Options to Eliminate Compilation Errors When Handling Checked Exceptions

- Use try-catch or declare exceptions using throws in the method signature.

## 24. How to Create a Custom Exception?

- Extend Exception class or its subclasses to create custom exceptions.

## 25. Handling Multiple Exceptions in a Single catch Block

- Separate exception types using the pipe symbol (|).

## 26. Explanation of try with Resources

- Automatically manages resources, closing them at the end of try block.

## 27. How does try with Resources Work?

- Automatically closes declared resources at the end of try block.

## 28. Exception Handling Best Practices

- Catch specific exceptions, provide meaningful error messages, log exceptions, and use try-with-resources for resource management.

