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







