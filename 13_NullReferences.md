## Null/nil references

### Java

- In Java, null can be assigned to any variable of a reference type.
```Java
Integer i = null;

if(i == null)
	System.out.println("it is null");
```

- Java does not implicitly check for null references. Instead, the developer has the responsibility to implements ways to handle null references. 
```Java
String hey;
List<String> stringList;
if (stringList == null) {
    stringList = new ArrayList<>();}
else if (hey != null) {
    stringList.add(hey);}
```

### Swift

- In Swift, the nil references is called Optional, which is a type that represents either a wrapped value or nil, the absence of a value.
```Swift
let number: Int? = Optional.some(42)
let noNumber: Int? = Optional.none
print(noNumber == nil)  // Prints "true"
```
