
####PyUnit

PyUnit is the Python equivalent of JUnit is Java which was written by Kent Beck and Eric Gamma. It is also called as unnittest. It is widely used for testing. The design on PyUnit is based on xUnit framework. Hence, we also find frameworks similar to it in C, Perl, Smalltalk, etc. 



![unittest module](http://twimgs.com/ddj/images/article/2014/0114/PythonUnitTest1.gif)

In the figure above, we see the unittest module. There are five key classes in unittest :

<p><b>TestCase :</b></p>
This class is used to create new test cases

<p><b>TestSuite :</b></p>
This class allows individual tests and test suites to be aggregrated

<p><b>TestLoader :</b></p>
This class is used to automate the process of creating a testsuite and populating it with individual tests.

<p><b>TextTestRunner:</b></p>
+ TestResults




 
As Figure 1 shows, there are five key classes in the unittest module. The TestCase class holds the test routines and provides hooks for preparing each routine and for cleaning up after. The TestSuite class serves as a collection container. It can hold multiple TestCase objects and multiple TestSuite objects.

The TestLoader class loads test cases and suites defined locally or from an external file. It emits a TestSuite object that holds those cases and suites. The TextTestRunner class provides a standard platform to run the tests. The TestResults class provides a standard container for the test results.

Out of these five classes, only TestCase must be subclassed. The other four classes can also be subclassed, but they are generally used as is.



Reference :

http://www.drdobbs.com/testing/unit-testing-with-python/240165163
https://docs.python.org/2/library/unittest.html#module-unittest
https://daringfireball.net/projects/markdown/syntax#precode
http://pythontesting.net/framework/pytest/pytest-introduction/
http://pyunit.sourceforge.net/

https://pymotw.com/2/unittest/


[NEXT](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/unittestcode.md)

[BACK]()
