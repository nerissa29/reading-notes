## Reading Notes: Intro to Big O Notation

The Big O Notation, according to Joshi (2017), is a "way of evaluating the performance of an algorithm". It's a way to express how much time a function, algorithm, or other actions, which based on the number of elements required to pass into that function, needs to run. Having a function that multiplies ten numbers is different from a function that handles multiplication of thousands or millions of numbers. This is where the Big O Notation comes in, it takes into the account both the speed and efficiency (Joshi, 2017).


<img width="515" alt="image" src="https://user-images.githubusercontent.com/113204667/208264071-774ee173-422d-4f8e-b25d-47cbaf0108f3.png">
Joshi, V. (2017). Basic Big O Notation Equations

### O(1) 

The **O(1)** is an algorithm that "always execute in the same time (or space) regardless of the size of the input data set" (Bell, n.d.). It will " always take the same amount of time and memory to run our algorithm" (Joshi, 2017). The amount of time and the amount of memory it needs to run the algorithm are the two important factor that needs to be considered.

Below is an example provided by Bell (n.d.):

```
bool IsFirstElementNull(IList<String> elements)
{
    return elements[0] == null;
}

```

### O(N)

The **O(N)** is where the algorithm linearly grows and is "proportion to the size of the input data set" (Bell, n.d.). This means that as the data or input grows, the time and space needed to run the algorithm grows as well (Joshi, 2017).



Reference:

Bell, R. (n.d.). A beginner's guide to Big O Notation. Rob Bell. https://robbell.io/2009/06/a-beginners-guide-to-big-o-notation

Joshi, V. (2017, January 23). What’s a linked list, anyway? [part 2]. Medium. https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996








