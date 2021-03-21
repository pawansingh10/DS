# Data Structure

## Data Structure
***
- Data Structure are fundamental concepts of computer science which helps us to write efficient program
- Organizing and storing data in a efficient form in the memory

### Differents types of Data Structure
***
* **1. Primitve Data Structure**
* **2. Non- Primitive Data Structure**

- **Primitve Data Structure**
  - Predefine way of storing data
  - |         |
    |----|
    | int     |
    | char    |
    | float   |
    | double  |
    
- **Non-Primitve Data Structure**
  - Derive from primitive data structure
  - **Linear**
   - |       |
     |-------|
     | Array |
     | Linkedlist |
     | Stack |
     | Queue |
     
  - **Non-Linear**
   - |         |
     |---------|
     | Tree |
     | Graph |
     | Binary Tree |
     | Binary Search Tree |
     
 ### Operation perform on Data Structure
 ***
   - Searching
   - Sorting
   - Insertion
   - Deletion
   - Updation
   
 ### Areas where Data Structure use
 ***
   - Manage large amount of Data Efficiently
   - Internet Indexing services provided by Google
   - Hierarchical Data Model - Tree
   - RDBMS - Arrays
   - Network Data Model - Graph
   
  
 ### **Array**
 ***
   - Collection of elements of Homogeneous Data types
   - Size is fixed
   - Occupy Contiguous Memory Location
   - Searching O(1) Constant time
   - Indexes start from 0 & ends with Size - 1
   
- **Operations**
   - |Searching|
     |---------|
     | Linear Search |
     | Binary Search |
   - | Sorting  |
     |----------|
     | Insertion Sort |
     | Bubble Sort |
     | Radix Sort |
     | Merge Sort |
     | Binary Sort |
   - | Insertion |
     |-----------|
     | Insert at start |
     | Insert at end 
     | Insert at any specific location |
     
   - | Deletion |
     |----------|
     | Delete at start |
     | Delete at end |
     | Delete at any specific location |
   
 - ```code
      int arr[5];
      |  1 |  2  |  3  |  4  | 
      |5000|           | 5010|
      arr[0]           arr[4]
      base address 5000
   ```
   
- **Advantages of Array**
   - Similar Data type Element
   - Random Access with the help of index value
   - Suitable When Size is knowned
   - Implement Stack and Queue
   
- **Disadvantages of Arrays**
   - Static Memory Location
   - Specify the time at compile time, **Not Dynamic**
   - Insertion and Deletion -> More Complex / Time Complexity
   - Due to this we can't implement the list using arrays
   
 
 
### **LinkedList**
***
   - In LinkedList, elements stores at any location in the memory instead of contiguous like array
   - As its name indicates, There is a **Link** between one one element and other element which is called **Node**
   - ```code
        | Data | Link |
            Node
       value    Add of next node
                  that's why not required contiguous memory
               
        
        | 10 I 1000 | --> | 20 I 2000| --> | 30 I 3000| --> | 40 I NULL|
          Head                                                 Tail
          start node                                           end node
     ```
     
 
- **Advantages of LinkedList**
   - No Wastage of Memory
   - No need to contiguous memory
   - Insertion and deletion, more simpler than Array
   - Stack and Queue can be implemented by using LinkedList 
   - Can Store any data types in Node
   
- **Disadvantages Of LinkedList**
   - Random Access not possible
   - Binary Search Algorithm is not possible because of no index value
   - Only forward traversal is possible
   - Reversing a Linkedlist is complex, because change all links of all nodes
   - Extra pointer Require to store address for each node
  
* **Singly LinkedList**
  - A LinkedList or Singly LinkedList is a set of nodes where each nodes has two fields, **Data** and **Link**
  - ```code
     Data              Link
     Actual value       add of next node
     
    ```

* **Doubly LinkedList**
   - Doubly linkedList contains an extra pointer or link typically called previous node address with the next node address and a data field like singly LinkedList
   - ```code
          | 500 |  A  | 1000 |
       prev add   data   next add
        
     ```
* **Circular LinkedList**
   - Linkedlist where all nodes are connected to form a circle
   - There is no NULL at the end
   - A Circular LinkedList can be a singly LinkedList or Doubly LinkedList
   - ```code
         | 2 | x |-->| 3 | y |--->| 3 | z |--->| 2 | x |
     ```
     
- **Advantage of Circular LinkedList**
   - Any nde can be starting point
   - Traverse whole list by start at any point, just need to to stop when the first value is revisited
   - Useful for Queue implementation, we don't need to maintain two pointers for Front and Rear if we use circular LinkedList
   - Real Time Example, **Operating System** manages all running application through circular linkedList to give each of them a slice of time quantum to execute
   - Circular Doubly Linked Lists are used for implementation of advanced data structures like Fibonacci Heap.
   - Circular linked list is the basic idea of round robin scheduling algorithm
   


### **Stack**
***
   - Linear Data Structure
   - All the elemets are arrange in a sequential manner
   - Follows **LIFO** Last in First Out approach
   - Example - Arranging Bread in a Packet

- **Operations**
   - **Push**  - Inserting an element on the top of stack
   - **Pop**   - Deleting an element from the top of stack
   
   > ***Both opertion are perform on the top of stack***
  
   > **Top = -1 indicates Stack is Empty**
   
 - | **Overflow Condition** | **Underflow Condition** |
   |------------------------|-------------------------|
   |         PUSH           |        POP              |
   | If we are trying to insert element to stack when stack is already have maximum element | If we are trying to delete an element from stack when stack is empty already |


- **Implementation**
   - Using Array
   - Using LinkedList










