modules and names

- module names are known from source, but only enter namespace at import
- qualified.entity
- import as , is alisaing
- dir(module) returns list of all etities in a module, if whole module was imported
- rem, at first import module is generated for additional semi-compliled ocde .pyc
- errors and exceptions, try something first, check if went ok, deal with exceptions
- multi branch excptions to giv ueful error code ouput


string revision

- immutable
- any changes result in a new string, eg assigned to the same name
- use id() to show actual object id
- string operations include replication and concatenation
- in and not in, easily used to find matching characters within a string
- (similar to finding strings in a list)
- strings do not have an append method or insert, and cannot use del[index] to remove characters
- so, due ot imutability, any major edits, e.g. additions via concatenation will just result in a new copy of the string, new object id, 
- even if referred to by the same name 
- 
- q's = how to tell if multiple edits and re-working of new strings wil impact code efficiency?
- min function  for strings, lists = finds the minimum "element" out of those in a sequence, can be alpabeticlaor numerical
- max() function, as above but for max values, 
- 
- .index method = - gives the character index within the string, of the first char of the passed in argument
- .count method = checks within a sequence (string, list) for nay occurences of test count argument, returns the number
- many other string methods: capitalize, center, endswith, isalnum (alphanumeric), title, 
- isalpha, islower, isspace, isupper, join, lower, lstrip, split, trip (combines rstip, lstrip, swapcase,
-  often both version that search from the left, or the right
-  .rfind(), .rstrip()    etc
- split method uses whitespaces to break up a string or tuple into seperate strings in a list
- 

sort and sorted

- sort method on a list just sorts the main list object
- sorted() functino created a new list object that holds the sorted results of the input list


st = 5.1.4.11     netc






