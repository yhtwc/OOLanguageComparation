## Functional programming

### Functional:
- All computation is the execution of mathematical functions
- Always returns the same output for a given input.
- Order of evaluation is usually undefined.
- No iteration, no for loop, no variable.
- Must be stateless. i.e. No operation can have side effects.

### Java
#### Does Java support Functional programming?
**Yes**. Java lambda expressions are new in Java 8. Java lambda expressions are Java's first step into functional programming. A Java lambda expression is thus a function which can be created without belonging to any class. A lambda expression can be passed around as if it was an object and executed on demand. Actually, Functional programming has been possible in Java since the introduction of anonymous inner classes.

Following is an example of showing using event handler with lambda expression
```Java
ChangeListener<Number> listener = (ObservableValue<? extends Number> observable, Number oldValue, final Number newValue) -> {
  renderBoard();
};
```

### Swift
#### Does Swift support Functional programming?
**Yes**. Closures are self-contained blocks of functionality that can be passed around and used in your code. Closures in Swift are similar to blocks in C and Objective-C and to lambdas in other programming languages. Thus, Swift also supports functional programming.

Following is an example of using Closures in swift, which is trying to find the first matched element in an array list.
```Swift
func world() -> Void { 
  print("Hello world!")
}
func hello(input_function: () -> Void) { 
  input_function()
}
hello(world)
```

