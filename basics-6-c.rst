- polymorphism = where a sybclass is able to modify its superclass
- therefore some "virtual methods" can be defined and redefined in superclasses can cause the behaviour of superclass to change
- class behaviour can be changed by subclasses
- example
- "abstract method" shows an ability or potential, that is then actually instantiated later by one of the subclasses
- polymorphism halps keep code clean and simple
- "composition" is another way to build up classes that are adaptable and well designed
- "composition" = composing an object by using other objects, building up by block sof code that can be added together in different ways
-compare and contrast inheritance vs composition
- inheritance works by extending the focus and abilities of a class (the class or subclass gives all the fuctionality)
- compositinn works by using classes as building blocs and adding them together to get the desired functionality (each class or subclass only gives part of the functionality)
- inheritance - single inheritance is easier, more safe, higher maintainability compared to multiple inheriance

- try except blocks
- try, except, else, finally
- finally blocks will always execute no matter what happens in the previous blocks

- exceptions are class
- exceptions can be caught, to allow the exception class object to be analysed
- any subclasses can be iterated over by using the __subclasses__()  method
- easy to create and use custom made exceptions (subclasses from existing exceptios)
 
- generators = code to produce a series of values and also to control the iteration
- closely links between iterators and generators
- function - invoked once and give a defined value
- generator - invoked several times (>1), gives a series of values
- iterators - conform to the iterator protocol
- iterators provide at least two methods, 
- __iter__()   returns the object itself, gets invoked once at the start
- __next__()  returns the next value in the iteration ..
- possible to create own classes that are iterators, if they follow the expected pattersn of iter and next
- custom iterators created in this are built up with functions, not subclassed

- yield, similar to return, but keeps the current state of the function, yield causes current stte of function to freeze, but able to be continued, from its current position
- yield can be used to build a function that acts as a generator
- including yield in a functino definition block turns it into a generator, rather than a normal function

- list comprehension -  allows lists and list contents to be built in situ without need for a full for loop structure, 
- listExample = [1 + numb for numb in range(10)]

- conditional expression as operator, check expression and evluates eg to T or F
- generators vs lists, always check object types
- notes within generators the entire list of all options never exists, whilst in list comprehensions a list object will occur, this will have memory implications
- listExample      = [1 if x % 2 == 0 else 0 for x in range(10)] 
- generatorExample = (1 if x % 2 == 0 else 0 for x in range(10)) 
- list comprehension within a tuple gives a generator
- square brackets = list comprehension
- parentheses = generator
- different design solution give same simple output, but in the context of different use cases, sped, memory use etc, one solutino may be preferable to another ...
