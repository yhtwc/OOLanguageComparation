## Errors and exception handling

### Java

- Java identifies three categories of Exceptions:
    - Checked Exceptions: An exception that occurs at the compile time; also called as Compile-time Exceptions.
    - Unchecked Exceptions: An exception that occurs at the time of execution. Also called as Runtime Exceptions.
    - Errors: These are not exceptions at all, but problems that arise beyond the control of the user or the programmer. 

- Java has an error and exception handling system by using a combination of the try and catch keywords. A try/catch block is placed around the code that might generate an exception. 
    - The code that may try to execute is placed in the try block. 
    - When an exception occurs, that exception occurred is handled by catch block associated with it. 
    - Every try block should be immediately followed either by a catch block or finally block.
    - A catch statement involves declaring the type of exception you are trying to catch. 

```Java
try {
// Protected code}
catch(ExceptionName e1) {
// Catch block
}
```

### Swift

- There are four ways to handle errors in Swift. 
    - Propagate the error from a function to the code that calls that function.
    - Handle the error using a do-catch statement.
    - Handle the error as an optional value.
    - Assert that the error will not occur.

```Swift
do {
    try expression
    statements }
catch pattern 1 {
    statements }
catch pattern 2 where condition {
    statements }
```
- Unlike most languages, error handling in Swift does not involve unwinding the call stack, a process that can be computationally expensive
