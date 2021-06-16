# Classes and Objects

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

You can create multiple different objects that are of the same class(have the same variables and functions defined). However, each object contains independent copies of the variables defined in the class.

[Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

# Thinking Recursively in Python

Problems (in life and also in computer science) can often seem big and scary. But if we keep chipping away at them, more often than not we can break them down into smaller chunks trivial enough to solve.

### The typical structure of a recursive algorithm:

 If the current problem represents a simple case, solve it. If not, divide it into subproblems and apply the same strategy to them.

 A _recursive function_ is a function defined in terms of itself via self-referential expressions. This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.

 A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure. List is not the only recursive data structure. Other examples include set, tree, dictionary, etc.

 [Thinking Recursively in Python](https://realpython.com/python-thinking-recursively/)

 # Python Testing with pytest: Fixtures and Coverage

### Fixtures

 When you're writing tests, you're rarely going to write just one or two. Rather, you're going to write an entire "test suite", with each test aiming to check a different path through your code. In many cases, this means you'll have a few tests with similar characteristics, something that pytest handles with "parametrized tests".

But in other cases, things are a bit more complex. You'll want to have some objects available to all of your tests. Those objects might contain data you want to share across tests, or they might involve the network or filesystem. These are often known as "fixtures" in the testing world, and they take a variety of different forms.

In pytest, you define fixtures using a combination of the pytest.fixture decorator, along with a function definition.

_Fixtures_ are used differently from global variables. For example, let's say you want to include this _fixture_ in one of your tests. You then can mention it in the test's parameter list. Then, inside the test, you can access the _fixture_ by name.

 Your fixture might act like data, in that you don't invoke it with parentheses. But it's actually a function under the hood, which means it executes every time you invoke a test using that fixture. This means that the fixture, in contrast with regular-old data, can make calculations and decisions.

You also can decide how often a fixture is run. For example, as it's written now, this fixture will run once per test that mentions it. That's great in this case, when you want to compare with a list or file-like structure. But what if you want to set up an object and then use it multiple times without creating it again? You can do that by setting the fixture's "scope". For example, if you set the scope of the fixture to be "module", it'll be available throughout your tests but will execute only a single time. You can do this by passing the scope parameter to the @pytest.fixture decorator:

```
@pytest.tixture(scope='module')

def example_function():
  blah, blah, blah...

```

 If your fixture has "module" scope, pytest will wait until all of the functions in the scope have finished executing before tearing it down.

 ### Coverage

When software gets larger and more complex, it's not going to be so easy to eyeball it. That where you want to have "code coverage", checking that your tests have run all of the code.

__So, how can you include code coverage with pytest?__ 

- Download and install a package called pytest-cov on PyPI

-  Once that's done, you can invoke pytest with the --cov option. If you don't say anything more than that, you'll get a coverage report for every part of the Python library that your program used, so I strongly suggest you provide an argument to --cov, specifying which program(s) you want to test. 

- Indicate the directory into which the report should be written. 

- Turn the coverage report into something human-readable. (I suggest using HTML, although other output formats are available)

 - This creates a directory called htmlcov. Open the index.html file in this directory using your browser, and you'll get a web-based report showing (in red) where your program still lacks coverage.

 [Python Testing with Pytest: Fixtures and Coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

 [<----- Back to About Me](../README.md)