# Java Exception Handling

This README provides brief answers to common questions about exception handling in Java.

## 1. What is Exception Handling in Java?
   - Exception handling in Java refers to the mechanism by which errors, or exceptional conditions, that occur during the execution of a program are managed and dealt with. It involves identifying, catching, and handling exceptions to ensure the smooth execution of the program.

## 2. In Java, what are the differences between a Checked and Unchecked Exception?
   - **Checked Exceptions:** These are exceptions that are checked at compile time. They must be either caught or declared using the `throws` keyword in the method signature. Examples include IOException, SQLException, etc.
   - **Unchecked Exceptions:** Also known as runtime exceptions, these exceptions are not checked at compile time. They can occur at runtime and are subclasses of RuntimeException. Examples include NullPointerException, ArrayIndexOutOfBoundsException, etc.

## 3. What is the base class for Error and Exception classes in Java?
   - The base class for both Error and Exception classes in Java is `java.lang.Throwable`.

## 4. What is a finally block in Java?
   - A finally block in Java is a block of code that follows a try-catch block. It is guaranteed to execute whether an exception is thrown or not. It is typically used for cleanup operations like closing resources.

## 5. What is the use of finally block in Java?
   - The finally block in Java ensures that certain code is executed regardless of whether an exception occurs or not. It is used for cleanup operations and releasing resources.

## 6. Can we create a finally block without creating a catch block?
   - Yes, it is possible to create a finally block without a catch block. A try block can be followed by either a catch block, a finally block, or both.

## 7. Do we have to always put a catch block after a try block?
   - No, it is not necessary to have a catch block after a try block. If a finally block is present, it can be used alone after the try block.

## 8. In what scenarios, a finally block will not be executed?
   - A finally block may not be executed if the JVM exits abruptly, such as in case of a system crash, or if there is an infinite loop or a `System.exit()` call within the try or catch block.

## 9. Can we re-throw an Exception in Java?
   - Yes, it is possible to re-throw an exception in Java using the `throw` keyword within a catch block.

## 10. What is the difference between throw and throws in Java?
   - `throw` is used to explicitly throw an exception within a method, whereas `throws` is used in the method signature to declare that the method may throw certain exceptions.

## 11. What is the concept of Exception Propagation?
   - Exception propagation refers to the process by which an exception is passed from one method to another until it is handled. If a method does not handle an exception, it is propagated to the calling method.

## 12. When we override a method in a Child class, can we throw an additional Exception that is not thrown by the Parent class method?
   - No, when overriding a method in a child class, the overridden method cannot throw checked exceptions that are not thrown by the parent class method. However, it can throw unchecked exceptions or no exceptions at all.
