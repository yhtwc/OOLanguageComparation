## Memory Management

### Java

- Java does automatic memory management which is implemented via garbage collection. Java Garbage Collection is the process to identify and remove the unused objects from the memory and free space to be allocated to objects created in the future processing.
- Basic Garbage Collection involves 3 steps:
	- Marking
	- Normal Deletion
	- Deletion with Compacting
- Advantage
	- It removes the burden of manual memory allocation/deallocation.
- Disadvatage
	- It effects the performance of the application.


### Swift

- Swift uses Automatic Reference Counting (ARC) to track and manage the memory usage. Whenever a variable holds an instance of a class, the memory count for that object increases by 1. If the variable goes out of scope or gets set to nil, the memory count decreases by 1.
- In most cases, ARC allows users to not think about memory management, it automatically frees up the memory used by class instances when those instances are no longer needed.
