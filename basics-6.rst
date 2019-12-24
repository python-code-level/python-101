start - 6

- python suitable for procedural and object based programming
- oop object oreiented programming
- objects have: name, individual properties, abilities to perform activties
- the large ficus tree grows quickly
- ficus = object name
- class = trees, or plants
- property = large
- activity = growth (quickly)

- methods are functions that are invoked from "within the data2, eg a class object or dataset can have a method that acts on it,  
- this contrasts to when data is "passed to" a function
- Procedural approach = seperate world of data, and world of code. Typically functions can use data, but data cant use functions.
- Object approach = both data and code are enclosed together in the same world, divided into classes

- Think of a class like a "recipe" - it can be used to create a useful "object" (by following the recipe) 
- Objects have traits = properties / attributes
- Every object has a set of traits and can perform a set of activites (methods)
- (module, file level function(), vs class.method)
- Objects are the incarnation of the ideas expressed within classes
- Properly constrcuted classes can prevent unauthorised or accidental misuse of data
- No clear boundary between data and code - they are combined togehter within objects
- 
- Classes (sub-classes) may be defined within an over-arching superclass 
- Class is a "set" of objects. Each object reflects the traits and qualitiies of its class. 
- Inheritance, anobject of one class with always inherit the traits, requirements and qualities of its superclasses

- All objects have: name, properties, activity
- OOP is essentially the art of designing, defining and expanding classes
- A class is simply a tool for creating relevant and suitable objects...
- Object is an instance of the class, created via instantiation


- Design plan - start with general and broad classes, then become more specific
- as soon as multiple instances may be required, then classes become useful... 

- Protect / hide values against mis-use or access = encapsulation, 
- __init__ is a constructor , invoked implicitly every time a new object is created from the class
- constructor needs to know all about the objects struture and will create all aspects on initialisation,  
- __init__ must have at least one parameter (self)
- self represents the soon to be created virtual object, so is a placeholder for future objects
- (using self is just a convention, but is best practice)
- So, any properties can be added to self, and they will be associated with any objects created 
- dot notation can access the property of the class object
- some properties can be locked to only internal use by the class, not externally accessible via n object...., this is encapsulation


class Stocks:
    def __init__(self):
        self.basePrice = 1.23
        
 stockObject = Stocks()
 print(stockObject.basePrice)
>1.23

class Stocks:
    def __init__(self):
        self.__basePrice = 1.23
        
 stockObject = Stocks()
 print(stockObject.__basePrice)
> AttributeError 

- Here the basePrice class component is private, only accessible within the class, not via an object,
- Using the .self means the method can access properties and methods of the object, 

- superclass and subclass
- in python it is necesssary to explicitly invoke the constructor of the superclass


class Stocks:
    def __init__(self):
        self.__basePrice = 1.23
        
 stockObject = Stocks()

class SubStocks:
    def __init__(self):
        Stocks.__init__(self)
        self.__sum = 0
        
 stockObject = SubStocks()


- instance variables are created by the constructorr and mean that different instances of a class may have different properties in thier isntance variables, depending on what processing has been done
- it is also possible to create properties of an object (class instance, on the fly, completely outside the class code and therfore also seperate from other instances of the class. 
-  
- Start at:
-  6.1.3.2
- in contrast to instance variables, which belong to an instance of the object, class variables just exist once and are stored in the class, so outside of any particular object
- so, even if no actual objects exist, or have been instantiated, the class variables will still exist
- using object.__dict__ can access instance variables of an object, but does not show the class variables
- the class variable can be accessed via any instance object of the class, but they will all show the same value.
- whenever a class variables is modified it is modified accross all instances of the class
- class dictionrary is used to access all info at the class level  ExampleClass.__dict__
- 
- the hasattr function can be used to check if any class or object has a certain property


if hasattr(egObject1, 'price'):
    print(egObj1.price)

if hasattr(egClass, 'cost'):
    print(egClass.cost)

- 





















