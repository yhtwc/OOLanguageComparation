## Properties

### Java
- Java does not treat "Properties" any different from "Member variables".
- Private member variables in Java can only be accessed using getters and setters, if outside the scope of the class definition. The 	   language does not have in-built support for default public getters and setters, and hence, require explicit declaration by the           developer. For example:
```java
public class Human {
    private String name;

    // Getter
    public String getName() {
      return this.name;
    }

    // Setter
    public void setName(String name) {
      this.name = name;
    }
}
```

### Swift

- A Swift property does not have a corresponding instance variable, and the backing store for a property is not accessed directly. This   approach avoids confusion about how the value is accessed in different contexts and simplifies the property’s declaration into a         single, definitive statement. All information about the property—including its name, type, and memory management characteristics—is     defined in a single location as part of the type’s definition.In addition to stored properties, classes, structures, and enumerations   can define computed properties, which do not actually store a value. Instead, they provide a getter and an optional setter to retrieve   and set other properties and values indirectly.
```Swift
class Temperature {
    var celsius: Float = 0.0
    var fahrenheit: Float {
    get {
        return (celsius * 1.8) + 32.0
        }
    set {
        celsius = (newValue - 32)/1.8
    }
    }    
}

var temp = Temperature()
temp.fahrenheit = 89
```
