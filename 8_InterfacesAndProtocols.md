## Interfaces / protocols

### Java
- Java support interface.
- An interface is a reference type in Java. It is similar to class. It is a collection of abstract methods. A class implements an interface, thereby inheriting the abstract methods of the interface.
- Along with abstract methods, an interface may also contain constants, default methods, static methods, and nested types. Method bodies exist only for default methods and static methods.

For declaring interface:
```Java
public interface Animal {
   public void eat();
   public void travel();
}
```
For using interface:
```Java
public class MammalInt implements Animal {
   public static void main(String args[]) {
      MammalInt m = new MammalInt();
      m.eat();
      m.travel();
   }
}
```

### Swift
- Swift Protocols are used in an identical manner as Java's Interfaces
- In Swift, a protocol can be adopted by a class, structure, or enumeration, to provide implementation of the required methods
- Protocol declaration involves using the keyword protocol. For example:
```swift
protocol MyProtocol {
    let hello = "Hello"
    var sayHello()
}
```
This can be implemented using the symbol : on a class declaration. For example:
```swift
public class MyClass : MyProtocol {
    func sayHello() {
        print(MyProtocol.hello)
    }
}
```
- The protocol can be used by initializing an object of the conforming class. A protocol cannot have its own instance. For example:
```swift
let myProtocol: MyProtocol = MyClass()
myProtocol.sayHello()
```

