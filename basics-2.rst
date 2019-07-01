# more python notes

key areas to define

- efficient way to define packages
- how packages relate together / to one another
- how many modules can fit in a package  
- 
- 

demo / test

- simple log files that updates when modules and methods within a package are imported


code creation and modules

- code decomposition, code can be decomposed into smaller component parts to keep them easier to maintain,  
- modules is one option to deal with the need for code decomposition
- many modules are pre-supplied as part of the python standard library
- the way a module is imported changes the way functions can be used
- imports obs must occur before the first use of a moduel function
- namespace = where anmes are uniqe, have meaning and do not conflict with one another
- inside a namespace, all names are unique,
- elements enter the namespace when they are qualified (not just when they are imported)
- import math
- math.pi
- math.sin
- this makes it very clear where the entities come from, and also means it is possible to have multiple pi or sin in a code, they only enter namespace when qualified by their source module
- it is also possible to do a selective import, so only use certain entities from a module, but can cause problems with name conflicts. any new definitions with same names will override previously imported entity
- from math import pi, sin
- from math import *
- the above generic way of importing all entities in a module has several drawbacks. mainly it can be unclear what exactly has been imported, and this can cause problems or conflict with functions in the main codebase
- a further option allows whole module to be imported with an alias, can help make it clear of a source module if conflicts or similar to existing modules, or can shorten the fully qualified names
- import numpy as np
- import pandas as pd
- a further option allows selected entities to be imported froma module and also aliased at the same time, 
- from numpy import leastcost as myleastcost, time as thistime  etc
- once using aliases the original names become unavailable


random number examples

- random module in python gives pseudorandom numbers
- so, data produced from programmed deterministic computers cannot be random?
- the modules work by taking a "seed" running the alogithm on that, then generating a new "seed value"
- many methods availabe, note alos in numpy
 
platforms, hardware and OS

- many methods, under platform to interegrate the underlying system architecture / platform

packages

- package is way of organising modules, bit like storage of files in a  directory folder
- whne python first imports a module, there is an elment of compilation that occurs,
- the pyc represents semi-compiled code, not actual machine code
- this process speeds up any other imports of the code
- setting any variable in a module allows it to be used elsewhere, after the module has been imported
- it is possible to warn users NOT to modify a variable, by convention, by using __variable
- it initialize a package, python will expect an init file to be located within the package root,
- whenever any of the packages modules are imported, the init file is executed, however it can be left empty (still essential)
- the main init file is required by the package at root location. however any subpackages can alos hold an init file, eg to add specialised functionality,   
- various ways to ensure packagesd and modules are available to program, one option is to append the location to the path, within the main file, then use "qualified package names", so, once the path has been set, modules or packages are imported relative to the root of the source files, eg the project directory,
- for multi nested packages, is very useful to use alias to import the last nested module
- in order to use storage efficiently, it is possible to zip a package from its root and thne import that by refering to it as if it were a directoy (pro = reduced storage, con = an additional step after / during coding and testing
- note, with a pipeline based development, all stages up to testing or pre=prod could use the main files, but once fully tested and accepted, a repo could set all master or prod packages to use the zip versions and delete the main source dir files 
 
exceptions /  raising an exception

- where an error or unexpected behaviour occur, python raises an exception
- the exception can be dealt with, in whcih case the program will procede
- alternatively an error message will be generated and the program will stop
- ideally software will be designed reasy to observe exceptions, identify them and then deal with them 
- try / except blocks allow code within the try block to run, then enact code within the except block wherever exceptions are raised, this allow code to progress neatly but can potentially hide some silently failing code unless it is well designed to handle potentila errors
- eg for calcs within a loop in the try block the loops stops and exists if an exception occurs, ,if behaviour wanted to continue analysis within the loop, then would need a try except block iside the for loop
- key issue with simple try / except blocks = is it possible that more than one exception error could occur
- if multiple except branches are used then if any are activated, it will cause the exception tobe caught and run, and no other blocks will be checked
- there are many groups of exceptions, in a nested tree, so that some exceptions are broad catch alls
- so wider, broad exceptions could be used to catch a range of potential problems, but note that with many exception blocks, any generic exception higher up would hide any lower downbut more specific exception, 
- it is possible to handle more thna one exception in the same way as others
- as well as catching exception in code, they can alos be raised
- raiseing and exception can help by testing to catch types of exception, 
- raise an exception can ensure the correct part of the codebase deals well with exceptions,
- simple raise exception routines can be used to help test code, with needingf to generte elaborate test data that cause actual tests to fail  
- assertions, these allow testing to assert if something is true, for example before code continues
- allows us to tests if the assertion has failed 
- using assert to catch errors help with debugging, or by being sure that data or objects sare of certain type or characteristics
- use of assumption can help make code more selef dopcumenting - explicit is better than implicit
- assert can be used to check, parameter types, values, data structures, situations that should not be allowed, or may cause errors, eg duplicate values etc,  
- assert allows the user or programmer to be very sure exactly why an error has arisen,
- very important to be clear how these help to accompany unit tests etc, by keeping these asserts close to a functino or object origin they keep code cleaner,  
- keep the origin and use of asers seperate from other key testing types     
- asserts can be turned off if needed during code compiling, eg once code builds are fully tested and stable?
- options for exceptions
- raise = allows an exception tobe raised, for checking, testing, logging or to correctly alert the user etc, 
- assert = check if certain conditions are true, then automatically raise exceptions if not
- try = the statements are executed until or if an exception is reached
- except = the exceptions are caught by these blocks, run through in order of listing, 
- else = code in this sectino runs if no exceptions in the except block ran, (like if, else)
- finally = this code will always run , whatever sequence of events has occured in the sections before it
- there are many types of useful exceptions, some include: memoryerror, overflowerror, lookuperror, 
- the key to using errors and exceptions well is the design of how they are thorwn and the way the information in them is caught and used


code inputs and character sets (encoding)

- ascii is most widely used character-number assignment
- american standard code for informatino interchange
- 256 chars
- code point is a number which makes (or translated to) a character, eg 65 = A
- code pages occur when blocks of code points (128 plus) are used for selected alphabet sets, even with the 256 restrictions of ascii
- so to resolve a code point, need to know both the code point vlaue and the code page
- unicode is an alternative method = it assigns unique characters to > million code points, 
- first 128 code points of unicode are the same as code point sin ascii, then diverges
- ucs-4 = universal character set, this uses four bytes / 32 bits to store each character (eg, the code point number)
- utf-8 = unicode transformation format, this more inteligently uses the correct amount of bits to store each code point
- python 3 supports unicode and utf-8 (re variable names etc, symbols, characters)
- so python 3 is now suitably for international use (I18N)
- 



























