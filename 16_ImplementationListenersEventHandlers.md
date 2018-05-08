## Implementation of listeners and event handlers

### Java

- In Java, event listeners represent the interfaces responsible to handle events. Common used event listeners are ActionListener, MouseListener, FocusListener and so on. There are `ActionEvents`. In order to receive an ActionEvent, a listener must implement the ActionListener interface and register itself with the component. Furthermore, a component must keep track of its listeners in order to notify them of an event.

```JAVA
class Event<T> {
    
    typealias EventHandler = (T) -> ()
    
    private var eventHandlers = [EventHandler]()
    
    func addHandler(handler: @escaping EventHandler) {
        eventHandlers.append(handler)
    }
    
    func raise(data: T) {
        for handler in eventHandlers {
            handler(data)
        }
    }
}
```

### Swift
- In Swift, ActionEvent is applied by using IBOutlet and IBAction associated with UI elements residing in Main storyBoard. Using listeners in Swift is to add willSet and didSet for the property. Putting them in a bracket after the property definition. willSet will be called automatically before the new value is set, and didSet will be called automatically after the new value is set. 

``` Swift
class Event<T> {

    typealias EventHandler = T -> ()

    private var eventHandlers = [EventHandler]()

    func addHandler(handler: EventHandler) {
      eventHandlers.append(handler)
    }

    func raise(data: T) {
      for handler in eventHandlers {
        handler(data)
      }
    } 
  }
```
