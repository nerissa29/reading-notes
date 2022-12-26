## Reading Notes: Class 05

### Implementation: Linked Lists

**Terminology:**

- **Linked List**
  - is a "data structure that contains nodes that links/points to the next node in the list" (Code Fellows, n.d.)
- **Singly**
  - signifies one reference that points to the *Next* node in the linked list
- **Doubly**
  - siginifies having two references within the node tat points to both *Next* and *Previous*
- **Node**
  - are "individual items/links that live in a linked list", each node containing the data for each link (Code Fellows, n.d.)
- **Next**
  - a property that contains reference to the next node
- **Head**
  - is a reference to the first node in the list (linked list)
- **Current**
  - a reference "to the node that is currently being looked at"
  - create a new **Current** variable at the **Head** when navigating, this ensures to start from the beginning of the linked list


**Traversal**

The *foreach* or *for loop* is not available when traversing.  The property *Next* shows us where the next node is. The *Next* value on each node helps us determine the next reference (or where the next reference is pointing). Tge *while loop* can be used when traversing; *while loop* can be used to check if the *Next* node is not null. The error *NullReferenceException* is shown when traversing into a *null* node; this will cause the program to crash.

The *Current* tells where we at exactly on the linked list and allows us "to move/traverse forward until we hit the end" (Code Fellows, n.d.). Below is a code example from Code Fellows. (n.d.):


```
"ALGORITHM Includes (value)
// INPUT <-- integer value
// OUTPUT <-- boolean

  Current <-- Head

  WHILE Current is not NULL
    IF Current.Value is equal to value
      return TRUE

    Current <-- Current.Next

  return FALSE"

```

**Traversal Big O**

- *for time*
  - it will be O(n)
  - for the node we are looking for could be the last node

- *for space*
  - it will be O(1)
  - when no additional space is required asid form what is already given







References:

Code Fellows. (n.d.). ***Linked Lists***. https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html

