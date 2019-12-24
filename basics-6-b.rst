- recap
- a class method is just a function that is within a class
- a method MUST have parameter >= 1
- so later on a method can be invoked without actually passing an argument, 
- but when it is first declared in the code it will always have at least one parameter, eg self

class Class:
    MAX = 99999 # A class constant, not expected to change
    variable = 9 #  A class variable, may change or be modified by code or analysis
    def aMethod(self):
        total = 100 # An object instance variable
        print('a message')
        print(self.variable)
        print(self.total)
        
    def anotherMethod(self):
        self.aMethod() # invokes the first method, when this method is called
        
object1 = Class()   # Instantiate an object of the class
object1.aMethod()  # Class the class method on the object

- self parameter is used to acess values of the object 
- self parameter can alos be used to invoke other class methods, within a class

- the __init__ method is a special type of method named a constructor
- it is called automatically every time an object is instantiated
- this allows wide range fo values, settings, param etc to be allocated to each indiv object
- the init method returns a new object not a value or calculation


- classes also have a built-in property of name, objects do not have a name property
- Class.__name__
- type can be used to find what class was used to instantiate a certain object
- cls.__bases__ shows the ancester for that class, eg from where it was inherited. 


- introspection = program's ability, at runtime, to examine an objects type and properties
- reflection = program's ability, at runtime, to change the properties and functions of an object

- string method, can be used to add a new default to print statement

def __str__(self):
    return self.values
    etc

- inheritance = whne methods and attributes are passed froma wider / broader / superclass 
- to a newer, more narrowly or specifically defined subclass
- instead of starting with a blank slate, the new class already has a base of functionality on which to build
- subclass inherits from superclass
- always possible to check if two classes are related, by using issubclass function
- important to note that a class is always considered to be a subclass of itself
- can use isinstance() to check what type of class a particular object belongs to
- however - important to note that this function will also return true when tested against any of an objects superclasses, 
- 
- obj1 is obj2 # tests if the two variables refer to the SAME object
- variables just store a handle pointing towards the internal memory location
- 
- the is operator tests if the pointers refer to the same object, whilst the == operator checks if the two variables show value equality
- the super() function accesses the superclass without the need to explixcirlt name it
- super() function allows easy access to resource, attributes etc inside the superclass


class Super: 
    supVar = 1 # class level variable
    def __init__(self):
        self.altSupVar = 100
    
class Sub(Super):
    subvar = 10 # class level variable
    def __init__(self):
    super().__init__()  # calls the init from super so altsupVar will also be accessible from Sub
    self.altSubVar = 999
    
obj = Sub
obj.subvar
obj.supvar

obj.altSupVar
obj.altSubVar


- it is clear that to access any property of an object, python searches both within the actual object, and also within all the classes to which the object belongs
- 
- start
- 6.1.5.12













- 
- 









