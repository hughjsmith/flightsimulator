# Developers Manual

## Stack.java
The class Stack is a collection of items. It uses a FILO policy to insert and remove.
Figure 1 shows the corresponding UML class diagram.

### Stack
- top
- counter
- Stack()
- push()
- pop()
- peel()
- isEmpty()
- size()

### Implementation
The attribute `top` represents the top of the Stack.
The attribute `counter` holds the number of items in the Stack.
The method `Stack()` is the constructor and initializes the state of the Stack.
The method `push()` adds a new item to the Stack. It expects the new value and does not have a return value. It increases the counter.
The method `pop()` removes an existing item from the Stack. It returns the removed value, and it does not have any parameters. It decreases the counter.
The method `peek()` returns the value at the top of the Stack and has no parameters.
The method `isEmpty()` returns a Boolean value that indicates if the Stack has any items. It returns true if the Stack is empty; otherwise, it returns false.
The method `size()` returns an integer value that indicates the number of items currently in the Stack. It returns zero if the Stack is empty.

### Usage
How do you create objects of the class Stack?

```java
Stack<Integer> stackofIntegers = new Stack<>();
Stack<String> stackofStrings = new Stack<>();
Stack<Flight> incomingFlights = new Stack<>();
```

Use the following code to add new items to the Stack

```java
IncomingFlights.push(flight);
```

Use the following code to remove an existing item from the Stack

```java
Flight flight = incomingFlights.pop();
```

## Queue.java
The class queue is a collection of items that uses a FIFO (First-in, First-out) policy to insert and remove.
Figure 2 shows the corresponding UML class diagram.

### Queue
- head
- tail
- counter
- Queue()
- enque()
- dequeue()
- peel()
- isEmpty()
- size()

### Implementation
The attribute `head` represents the front of the queue (first item in the line)
The attribute `tail` holds represent the back of the queue (last item in the line).
The attributor `counter` holds the number of items in the queue.
The method `Queue()` is the constructor and initializes the start of the queue.
The method `dequeue()` removes an existing item from the queue; items always leave at the front of the queue. It returns the value, and it does not have any parameters. It decreases the counter.
The method `enqueue()` adds a new item to the queue; new items always join at the back of the queue. It expects the new value but does not have a return value. It increases the counter.

### Usage
To create a Queue, use the Queue constructors and indicate the following data type for the items.

```java
Queue<Integer> queueofIntegers = new Queue<>();
Queue<String> queueofStrings = new Queue<>();
```

Use the following to create a queue of flights.
Use the following code to add a new item flight into the queue.
Use the following code to move an existing item (flight) from the queue.

## List.java
The class List is a collection of items. It keeps all items in ascending order. Figure 3 shows the corresponding UML class diagram. The class List is a collection of items. It keeps all items in ascending order. Figure 3 shows the corresponding UML class diagram.

### List
- First
- last
- Iterator
- counter
- List()
- insert()
- moveToFirst()
- movetoLast()
- movetoPrev()
- getData
- hasData
- isEmpty
- size()
- toString()

### Implementation
The attribute `first` represents the first item in the list. It is the smallest item in the list.
The attribute `last` represents the last item in the list. It is the largest item in the list.
The attributor `iterator` represents the current item in the list. It moves through the entire list. It can move forward and backwards.
The attributor `counter` holds the number of items in the list.
The method `insert()` adds a new item to the list; new items always join in order. Those methods expect a new value that does not have a return value; it also increases the counter.
The method `movetoFirst()` moves the iterator to the first item in the list.
The method `movetoLast()` moves the iterator to the last item in the list.
The method `move to next()` moves the iterator to the next item in the list
The method `movetoPrev()` moves the iterator to the previous item in the list; use this method to move backwards in the list
The method `getdata()` returns the item pointed by the current iterator
The method `hasdata()` returns true if the current iterator points to a valid item in the list; otherwise, it returns false.
The method `isEmpty()` returns a Boolean value that indicates if the list has any item it returns.
The method `size()` returns an integer value that indicates the number of items currently in the list; it returns zero if the list is empty.

### Usage
To create a list, use the list constructor and indicate the data type for the target items as follows:

```java
List<Integer> listofIntegers = new List<>():
List<String> listofString = new List<>();
```

Use the following code to add a new item (flight object) to the list.
Use the following code to loop through a list of flights where buffer is an output file:
Use the following code to print all the content of the list

```java
System.out.print.ln(landedFligths.toString());
```
```
