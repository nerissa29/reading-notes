## Reading Notes: Class 02

### Testing and Modules

#### In Tests We Trust — TDD with Python

Gomes (2017) stated that **unit tests** are "some pieces of code to exercise the input, the output and the behavior of your code", it can be written at any time. However, the strategy to think and write is called the **Test-Driven Development**. TDD is a development of tests (testing a feature); it is advisable to run tests before adding that feature to your code.

For example, if you developed an API connection that identifies possible genders, the code needs to return the possible gender as the output (once the name is entered). Therefore, writing a test is important, meaning writing a code/function to test it. The **test name** must state "what is expected and what we are testing" (Gomes, 2017).

The author, Gomes, also mentioned in her article that the **test file** should "follow the same name of module name", so if the module is named *first_module.py*, then the **test name** should be *test_first_module.py*.

```
module/
- first_module.py

tests/
- test_first_module.py

```

Another important thing to consider is the structure, and one of the widely used is the **AAA (Arrange, Act, and Assert)**. Gomes (2017) describes *AAA* as follows:

- **Arrange** - organizing the data needed to execute the input, for example, or any piece of code
- **Act** - executes the code that is being tested
- **Assert** - once the code is executed, always check if the output or result meets what is expected

Once all these three are ready, the tests can be executed using **pytest** (or any other).

#### The Cycle

The cycle's three steps (Gomes, 2017): 

- write a unit test; it should fail because the feature is not there yet
- write the feature; this will make the test pass
- refactor the code

This cycle can be repeated every time a feature is added or modified.

Below is an image example of the code and test run (Gomes, 2017): 

<img width="511" alt="image" src="https://user-images.githubusercontent.com/113204667/208487361-82b560b4-7b1b-42fb-bd2d-9a4d60d08881.png">

Gomes (2017) also provided two books that contain information about TDD:

- [Test Driven Development: By Example](https://www.amazon.com.br/Test-Driven-Development-Kent-Beck/dp/0321146530)
- [Growing Object-Oriented Software, Guided by Tests](https://www.amazon.com.br/Growing-Object-Oriented-Software-Guided-Tests/dp/0321503627)


### What does the if __name__ == “__main__”: do?

The __name == "__main__" will execute the code when the file runs as a script and not when imported as a module. The python interpreter reads the source file before executing the code and defines special or global variables before executing (Shah, (n.d.)). If that module or source file is what the python interpreter runs as the main program, then "it sets the special __name__ variable to have a value “__main__” " (Shah, (n.d.)).

However, if the file is imported from a different or another module, then the __name__ will be set to that module's name (Shah, (n.d.)). In her article, Shah (n.d.) describes 










References:

Gomes, A. (2017, September 14). *In tests we trust — TDD with Python*. Code Like A Girl. https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932

Shah, N. (n.d.). *What does the if __name__ == “__main__”: do?*. Geeks for Geeks. https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/




.................

Freitas, N. (2015, January 6). *People around the world are voluntarily submitting to China’s Great Firewall. Why?* Slate. http://www.slate.com/blogs/future_tense/2015/01/06/
tencent_s_wechat_worldwide_internet_users_
are_voluntarily_submitting_to.html


