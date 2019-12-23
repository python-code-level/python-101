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


```class Stocks:
    def __init__(self):
        self.basePrice = 1.23
        
 stockObject = Stocks()
 print(stockObject.basePrice)```

class Stocks:
    def __init__(self):
        self.basePrice = 1.23
        
 stockObject = Stocks()
 print(stockObject.basePrice)

























