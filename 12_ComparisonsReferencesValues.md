## Comparisons of references and values

### Java

- In Java, "==" is used to compare references.
```Java
int x = 1;
int y = 2;

if(x == y)
	System.our.print("there are the same");
else
	System.our.print("there are not the same"); //Print this
```

- The .equals() method is used to check whether two references both refer to the same value.
```Java
String string1 = new String("John");
String string2 = new String("John");
String string3 = string2;

if(string1 == string2)
	System.our.print("there are the same");
else
	System.our.print("there are not the same"); //Print this

if(string1.equals(string2))
	System.our.print("there are the same"); //Print this
else
	System.our.print("there are not the same");

if(string2.equals(string3))
	System.our.print("there are the same"); //Print this
else
	System.our.print("there are not the same");

if(string1 == string3)
	System.our.print("there are the same"); //Print this
else
	System.our.print("there are not the same");
```

### Swift

- In Swift, "==" is used to compare value.
```Swift
var aString = "123"                            // "123"
var bString = (aString as NSString)            // "123"
aString == bString                             // true, content equality
aString === bString           		       // error
```

- In Swift, "===" is used to compare references.
```Swift
var st1 = NSString(string:st)                  // "123"
var st2 = st1                                  // "123"
st1 === st2                                    // true
```
