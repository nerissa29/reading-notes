## Reading Notes 1

### Intro to Big O Notation

The Big O Notation, according to Joshi (2017), is a "way of evaluating the performance of an algorithm". It's a way to express how much time a function, algorithm, or other actions, which based on the number of elements required to pass into that function, needs to run. Having a function that multiplies ten numbers is different from a function that handles multiplication of thousands or millions of numbers. This is where the Big O Notation comes in, it takes into the account both the speed and efficiency (Joshi, 2017).


<img width="515" alt="image" src="https://user-images.githubusercontent.com/113204667/208264071-774ee173-422d-4f8e-b25d-47cbaf0108f3.png">
Joshi, V. (2017). Basic Big O Notation Equations

#### O(1) 

The **O(1)** is an algorithm that "always execute in the same time (or space) regardless of the size of the input data set" (Bell, n.d.). It will " always take the same amount of time and memory to run our algorithm" (Joshi, 2017). The amount of time and the amount of memory it needs to run the algorithm are the two important factor that needs to be considered.

Below is an example provided by Bell (n.d.):

```
"bool IsFirstElementNull(IList<String> elements)
{
    return elements[0] == null;
}"

```

#### O(N)

The **O(N)** is where the algorithm linearly grows and is "proportion to the size of the input data set" (Bell, n.d.). This means that as the data or input grows, the time and space needed to run the algorithm grows as well (Joshi, 2017).


Below is an O(N) example provided by Bell (n.d.):

```
"bool ContainsValue(IEnumerable<string> elements, string value)
{
    foreach (var element in elements)
    {
        if (element == value) return true; 
    }     
    return false; 
}"

```

#### O(N2)

The **O(N2)** describes an algorithm that runs correspondingly to the square size of the input (Bell, n.d.). This algorithm takes more time and memory to run, depending on the number of inputs or data sets (Joshi, 2017).

An example of O(N2), provided by Bell (n.d.):

```
"bool ContainsDuplicates(IList<string> elements)
{
    for (var outer = 0; outer < elements.Count; outer++) 
    {
        for (var inner = 0; inner < elements.Count; inner++) 
        { 
            // Don't compare with self 
            if (outer == inner) continue;             
            
            if (elements[outer] == elements[inner]) return true; 
        }
    }    
    return false;
}"

```

#### O(2^N)

According to Bell (n.d.), the **O(2^N)** describes an algorithm that doubles its growth "with each addition to the input data set". One good example are recursive functions, such as the Fibonacci sequence/function.


Below is the Fibonacci function example, provided by Bell (n.d.):

```
"int Fibonacci(int number)
{
    if (number <= 1) return number;
       
    return Fibonacci(number - 2) + Fibonacci(number - 1); 
}"

```


### Names and Values in Python

Below are some facts regarding names and values in Python, according to Batchelder (2015):

- "Names refer to values"
- "Many names can refer to one value"
- "Names are reassigned independently"
- "Values live until no references"
- "Assignment never copies data"
- "Changes are visible through all names"
- "Mutable Aliasing"
- "Immutable values can't alies"
- "Change is unclear", includes:
  - rebinding variable
  - mutating, such as used of .append() on list
  - rebind lists
- "Mutable and immutable are assigned the same"
- "Assignment Variants", such as:
  - x += y  >>>  same as x = x + y
- "References can be more than just names"
  - an example would be *list elements*
  - object attributes
  - variable names (left-side of the assignment, name = "Issa")
  - Dict (Dictionary) values
- For-loops
  - iterates over the elements/sequence
- "Function arguments are assignments"
  - parameters match the arguments
- Any name can refer to value at any time
- Names have no type but have a scope, values have no scope but have a type

Myths on Python according to Batchelder (2015):

- "Python has no variables"
- "Call-by-value or call-by-reference?"
- "Making a 2D list"





Reference:

Batchelder, N. [PyCon 2015]. (2015). Ned Batchelder - Facts and myths about Python names and values - PyCon 2015. [Video]. YouTube. https://www.youtube.com/watch?v=_AEJHKGk9ns

Bell, R. (n.d.). A beginner's guide to Big O Notation. Rob Bell. https://robbell.io/2009/06/a-beginners-guide-to-big-o-notation

Joshi, V. (2017, January 23). What’s a linked list, anyway? [part 2]. Medium. https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996

