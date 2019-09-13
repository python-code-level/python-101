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
* so varied use of assert through system code can give extra assurance, anbd help to raise meanginful error at set points

types

* common useful exceptions = ArithmeticError, AssertionErro, IndexError, LookupError, 
* MemoryError, 

5.1.7.1

text and inputs

* I18N = internationalisation
* ascii defines character sets by numbers
* code point is a number which makes a character
* code page standard uses dif code points for certain national language characters
* unicode assigns unambigious chars to many man y code points (avoids need for code pages)
* useful standard is UTF-8 unicode transformatino format 
* unicode / UTf-8 encoded chars can be used for variable names etc in python
7 so python 3 is I18N ed

5.1.8.1

basic revision

* strings, immutable sequences, so have length and cnabe indexed
* multiline by three apostrophes or triple quotes
* concatenated or replicated
* can be sliced like lists or arrays
* true or false results from using in and not in for strings and subsets
* cant think exactly of string being like a list, as stringis immutable
* no append, no insert, 
* modifications to strings are always new copies, 
* strings have an index method - gives the first occurence of the argument
* count method, counts element occurences in the string sequence
* other common methods ...   .endswith()  find() .replce() etc, etc, 

5.1.10.3

string sorting

* sorted function vs sort methodf 

start - 6

* python suitable for proceduarl and object based programming 
* objects have: name, individual properties, abilities to perform activties
* the large ficus tree grows quickly
* ficus = object name
* class = trees, or plants
* property = large
* activity = growth (quickly)






