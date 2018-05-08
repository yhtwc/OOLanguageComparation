## Classes

### Java
- Classes can be defined in Java using the keyword class. For example:
```java
public class Dog {
   String breed;
   int age;
   String color;

   void barking() {
   }
   void hungry() {
   }
   void sleeping() {
   }
}
```
- Instances require a constructor. Every class has an implicit empty default constructor. Explicit default constructor or parameterized constructor can be defined if needed, using access specifier and class name. For example:
```java
public class Animal {
   String type;
   String color;

   // Explicit default constructor
   public Animal() {
     this.type = "Bird";
     this.color = "Blue";
   }
   // Explicit parameterized constructor
   public Animal(String type, String color) {
     this.type = type;
     this.color = color;
   }
}
```

### Swift

- **Swift** are building blocks of flexible constructs. Similar to constants, variables and functions the user can define class   	   properties and methods. **Swift** provides us the functionality that while declaring classes the users need not create interfaces or     implementation files. **Swift** allows developers to create classes as a single file and the external interfaces will be created by     default once the classes are initialized.
```swift
class student{
   var studname: String
   var mark: Int 
   var mark2: Int }
let studrecord = student()
class MarksStruct {
   var mark: Int
   init(mark: Int) {
      self.mark = mark}
}

class studentMarks {
   var mark = 300}
let marks = studentMarks()
println("Mark is \(marks.mark)")
```
