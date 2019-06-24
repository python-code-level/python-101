Python basics (background for exam prep)

Summary review and reminders

- scalar, a data type that has a single value
- natural numbers and factorials
- recursion
- 

Main topics

- Commands, Instruction list (IL) = complete set of the known commands
- similarities between natural languages and machine languages
- contains: alphabet, dictionary/lexis, syntax rules (is it valid?), semantic rules (does it make sense?)
- instruction list (IL) is similar concept to the machines "alphabet2
- high level programming languages help communicate between underlying basic commands and instruction list and human language
- machines execute machine code, but programs written for high-level programming language are "source code" and contained within a source file
- for program to work as expected and designed, needs correct commands / alphabet, correct lexix / dictionary, correct syntax, and correct seamtnically
- when ready for use, program needs to be rednered into machin elanguage
- two main methods to convert from hig-level programming language into machin elanguage - compilation and interpretation
- compilation is translated / compiled once, to create the file that can be executed (the machine code file)
- interpretation, the translation happens each time the code is run , so the prgram code always needs an interpreter for it to run. eh directly sharing just the code will not work in the absence of a suitable interpreter.
- an interpreter translates source text file code by reading top to bottom and left to right, the interpretor also checks the code to see if it is functional before it is executed, (read-check-execute), the interpretor thows an error if the code cannot be executed (if fails any checks)
- note that the interpreter can move through large amounts of the code befor eit may find an error and stop the execution, eg its begisn the process then stops, rather than fully chekcing everyting first
- different pros and cons for each type of programming language
- compilation - pros = executes fast, does not need the compiler to be shipped with the code, quite a secure and read protected method, eg difficult to view and read the code if people wanted to (as it is just in machine code)
- compilation - cons = can be slow to compile and therefore difficut to do quick code - test fedback loops, may need multiple compilers to fit a rang eof user hardware
- interpreted - pros = quick to just run and test code straigth away - quick feedback loops, code storage is via text files of progamming language code, not machine code, the code is converted later at poin tof use, so is more adaptive to whatever run environment or hardware it is being run on
- interpreted - cons = code can be slow, as resources are shared with the interpreter when it is used, both developers and end users need access to an appropriate interpreter,
- python = interpreted language, therefore to run a python program, need access to installed python interpreter, 
- often interpreted languages refered to as scriptin glanguages, with text files being "scripts"
- dev by Guido van Rossum, netherlands
- Stated goals for the developement of python include: easy, intuitive, but powerful, open source, understandable code (c.f. plain english), small task suitable, short dev times. 
- Several features of python make it popular:  considered easy to learn and use, favoured for teaching, free, understanable, 
- most similar languages: perl, ruby

ongoing evolution

- python 3 is now current and is essentially a different, updated language compared to python3, although much in terms of use is similar
- important to note there are many different flavours of python
- python software foundation releases the main reference python versions (CPython, note, !=, c.f. Cython!)
- these key releases are written in C. 
- note benefit of C origin is portability, due to ubiquity of C
- Cython, this automatically converts python code to C code, therefore it speeds up the analysis / calculations
- jython, this acts as a link between java and python
- pypy, is a fast, compliant implementation of python, its main advantage is speed. it is built with RPython (can be considered as a toolfor python developers, i.e. developers of python, than users)

terminology

- traceback - shows the route the code takes and locations where errors or issues occur, 
- erors have specific names, due to types
- function = sectionof code that causes an effect, or undertakes evaluation, gives a result (python has many "built-in" functions, but also can be witten or imported
- python function takes one, o rmany arguments function(argument1, argument2)
- function invocation 

rules / process / reminders

- only one instruction per line of code
- \ backslash as an escape character
- positional - the meaning of an argument is determined by its position
- keyword arguments - the meaning / selection of the argument is shown by the keyword
- keyword arguments are always placed AFTER the last positional argument 

literals

- data added as a constant or a variables = several types of "literals"
- you can literaly tell what it is by examining the data
- literals are defined by the type of datsa they hold
- literals are used to encode data
- literals relate to data type, and how these are stored in memory
- note decimal, octal, hexidecimal integers
- octal is base8
- decimal is base10
- hexadecimal is base 16
- floats , floating point have non-empty decimal fraction
- scientific notation is supported
- python uses the most economical representation for numbers that is available 
- e.g. python choose scientific notation for long or complex numnbers, where relevant

rules

- recall that hierarchy of priorities applies
- operation of higher priority are performed first and passed to lower priority operations
- left sided binding normally applied where priorities are otherwise equal
- important - the exponentiation operator uses right-sided binding (righ associative)
- BODMAS
- Brackets (inside brackets first).
- Orders (powers or square roots).
- Division.
- Multiplication.
- Addition.
- Subtraction
- note, any parts of expressions - in parenthese are calculated first

python ordering: operator priority (high to low)

- +- unary
- ** 
- * / %
- + - binary
- <<   >> binary shift 
- < <=>>> >=
- ==  !=
- &
- |
- = (many)


variables

- a container, where the contents can be varied
- name and value
- name must not clash with builtin researved keywords
- must begin with letter ansd have no specila characters, except underscore, no spaces
- very flexible - content type can change and alter
- created when values are assigned
- the assignment operatoris = 
- names should ideally be self-commenting

shortcuts

- shortcut rule
- variable = variable op expression
- can be replaced by
- variable op= expression
- e.g. var = var / 2 becomes var /= 2
- e.g. var = var + 1 becomes var += 1

reserved keywords

- False, true, None
- while, from, not, in, del, and
- with, r, as, elif, global
- if, else, pass, yield, break, assert
- raise, return, try, class, def, continue
- finally, exce, import, except, lambda


functions

- names should ideally be self-commenting
- various built in functions- 

questions and equality

- == compares to see if true
- == a binary operator with left-sided binding

conditional instruction / conditional statement: for loops, while loops

- if true_or_not:
      do_this_if_true()
- while i < number:
     do_this()
     modify i 
 

break and continue KEYWORDS

- syntactic candy / syntactic suagar = can make a developer's work easier, but might not strictly be essential in a programming language
- break = exists the loop by leaving the loop body of code. file code execution continues at the next command outside the loop
- break is used once a point has been reached that no further use of the loop is needed. 
- continue = 
- continue is used where the loop needs to be reset, and a part of the calculatino omitted or skipped, eg it moves tothe next iteration in the loop without acting on the current

loop-else

- not widely recommended to use
- eg can be difficult to read, may be better to use alternatives, e.g. next(), filter()

Review and add to notes

- while loop, statements are executed when a conditional is met
- for loop, moves over an iterable, can be combined with range
- the flow and exit points of a loop are modified via break (stop) and continue (skip)
- range(start, stop, step)

logical operators

- conjugation = connection of seperate conditions (and)
- disjunction = compound action that depends on at least one operation / statement (or)
- logical negation = 

De Morgan's law
The negation of a conjunction is the disjunction of the negations
not (p and q) == (not p or (not q)

the negation of a disjunction is the conjunction of the negations
not (p or q) == (not p) and (not q)

logical vs bitwise operators

bitwise operators

& (ampersand) bitwise conjution
| (bar) bitwise disjunction
~ (tilde) bitwise negation
^ (caret) bitwise exclusivce or (xor)

Arguments for bitwise operators must be integers, not floats (so may need to be converted)

bitwise operators can be used to check the value at a specific point in a bit image
such an example (grab a value, or change selected bits) = bit mask

digraphs indicate "shift operators" 

variable types

- scalar variables (store one given value at a time)
- multi-value variables 

cards

listnumbers = [1,4,8,16]

- list is adata type, mutable, can be ordered
- "elements" in a list are numbered, starting from 0
- list is a collection of elements, where the elements are scalars
- find elements via indexing, listnumers[1]
- len(list) = number fo elements stored within the list
- del(list[index]) removes element from list
- list, access by index[2] and negative index[-3] -1=last in the list
- common methods, list.append(0), list.insert(1,245)
- lists can be iterated over element by for loops wiht "in"
- name of a list refences the memory locatino where the list is stored, 
- different list names can relate to the same memory location
- slice , makes a copy of a whole list, or selected part of a list
- list slice list[:] copies all,  or list[start:end]
- list[0:end]  is same as list[:end]
- list[start:] is same as list[start:len(list)]
- del can delete slices from a list
- "in" 
- list comprehension 
- [expression for element in list if conditional]
- for element in list:
      if conditional:
          expression

multidimensional arrays related to lists 

functions and methods

- functions relate to code as a whole
- method is a type of function
- method acts, and is invocated in specific ways
- method changes the state of an entity
- method is tightly linked / owned by the data on which it acts
- the data "owns" the method
- method chnages the internal state of data on which it is invoked

resultoutput = function(param1, param2)
resultoutput = data.method(param11, param2)

cards done up to here
start 

functions
- help to avoid repition of code by allowing re-use, encapsulation of code
- functions add clarity to long sections of code analyssi, help improve readability and flow
- the coding problem should be broken into small pieces, and each captured into a function
- decomposition of a problems into seperate functions
- make it much easier to test code gradually in small sections / isolated sections
- aim is to divide code up into easy to access and understand functions 
- functions aslo assist whne multiple developers are working on the same project
- functions from python built-in, imported modules, local code
- define a functino with def !
- function is invoked, body of the function is executed, 
- function must be available, accessible before it is invoked
- functions should not have the same name as variables
- return keyword cause function to exit immediately
- return can complete epty, or can return an expression/variable
- return with expression cause the expression to be evaluated at the end of the function
- functions can have both effects and results, wont always need to use both in further calcs
- None is a keyword, but cant occur in expressions
- None is used, when it is assigned to a variable, , or whne it is compared to a variable
- when return is used without an expression, it returns None

parameters vs arguments
- parameter = specialised variable
- parameter only exists within a function def(parameter)
- the actual value of the parameter (because it can be different each time) is passed to the parameter when the method is invoked, and when, during invocation, an argument is passed to the method
- "the result of the argument is the parameter value" 
- "you can hear the argument outside, but only the paramters live inside (the function)"
- shadowing, inside a function any parameter with the same name as a variable outside the function will shadow that variable, and be used in preference, but nothing outside the functino has been reset, outside the functino the other main parameter still takes preference 
- how many parameters can be used before a method is too complex?
- positional vs keyword argument passing (passed from argument outside to parameter inside)
- a function can be set so that is certain arguments are not passed in, then default values are used,
- so essentially predefined values for a parameter are set, as if the argument had been passed in

summary of function arguments (outside) to parameters (inside)
- positional , depends on the order that arguments are supplied to the function
- keyword - defined and triggered by their keyword
- default , when no associated argument exists, a predefined parameter values is used

scope
- scope of a name, variable, is the part of the code where the name is properley recognizeable  
- c.f. parameters, they are only accessible within a function, that is their scope
- any variable defined outside the function, is still accessible within the functiln, not vice versa
- however if the variable outside the functino get replaced, by shadowing, by a variable inside the functino, then not the case
- the global keyword can be used to change behaviour within a function to allow variables to be modified outside the function scope  
- changes to a list identified by the functino parameter will be reflected beyond the scop eof the function
- functions can see and use variables from the wider code body, unless a variable is being shadowed by an internal function var

recusrion

- w 
- 

































