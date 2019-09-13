5.1.5.1

exception - when they occur, force the output of an error message
* many types of exceptions, from general to very specific
* hierachy tree of related exceptions
* also possible to create new exception types, by subclass of exception class
* Exception, is one level "up", or more specific than BaseException
* so, can catch a whole group of possible exceptions by using a more generic exceptino catch
* order, and general / specific are important whne creatin glists of exceptions
* can handle more than one exception at a time, by putting in a list
* need to consider and decide - deal with exception inside function, or outside function, eg where they are called?

raise
* keyword to cause a specified exception to occur
* note, how to test that error and exceptions are dealt with correctly by a system? A = can be dealt with by raise, as a strategy
* key use is seperating the areas where an exception is handled from where it is generated- 

assert and assertion error
* if assertion fails, ie is not true, then exceptino error is raised
* can help to verify that data or code steps are exactly as expected ..
* consider as a useful supplement to using exceptions ...




