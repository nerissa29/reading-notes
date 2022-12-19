## Reading Notes: Class 02

### Testing and Modules

#### In Tests We Trust — TDD with Python

Gomes (2017) stated that **unit tests** are "some pieces of code to exercise the input, the output and the behaviour of your code", ot can be written at any time. However, the strategy to think and write is called the **Test-Driven Development**. TDD is a development of tests (testing a feature); it is advisable to run tests first before adding that feature into your code.

For example, you developed an API connection that identifies possible genders, the code needs to return the possible gender as the output (once name is entered). Theerefore, it is important to write a test, meaning write a code/function to test it. The **test name** must state "what is expected and what we are testing" (Gomes, 2017).

The author, Gomes, also mentioned in her article that the **test file** should "follow the same name of module name", so if the module is named *first_module.py*, then the **test name** should be *test_first_module.py*.

```
module/
- first_module.py

tests/
- test_first_module.py

```

Another important thing to think about is the structute, and one of the widely used is the **AAA (Arrange, Act, and Assert)**. Gomes describes *AAA* as follows:

- **Arrange** - organizing the data needed to execute the, input for example, or any piece of code
- **Act** - executes the code that are being tested
- **Assert** - once the code is executed, always check if the output or result meets what is expected

Once all these three are ready, the tests can now be executed using **pytest** (or any other).

#### The Cycle

The cycle' three steps (Gomes, 2017)




References:

Gomes, A. (2017, September 14). *In tests we trust — TDD with Python*. Code Like A Girl. https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932




.........
Freitas, N. (2015, January 6). *People around the world are voluntarily submitting to China’s Great Firewall. Why?* Slate. http://www.slate.com/blogs/future_tense/2015/01/06/
tencent_s_wechat_worldwide_internet_users_
are_voluntarily_submitting_to.html


