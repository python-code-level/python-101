- some streams are already available, these are stdin, stder, stdout
- available via import sys
- sys.stdin = standard input,  this default to keyboard input
- input() reads data from stdin by default
- stdout = stadard output, defaults to screen ouput
- print() is default to output data to the stdout stream
- stderr = standard output error, defaults to screen
- these default streams can be accessed and re-directed, they dont explicitly need closing
- streams are closed by stream.close()
- stream errors can be captured in a try catch block, 
except IOError as exc:
  print(exc.errno)
- errno returns the error number
- also general Exception can be passed to functino to prin tout its string
- eg.g

from os import strerror
except Exception as exc:
print(strerror(exc.errno))

- note the dangers of reading in a whle file if it has unknown content or length- 
- eg read will be memory dependant, 
- stream.read(), vs stream.readline()
- stream.readlines() reads all the file, but returns a list, with one line per item, 
- the file object from open() is an iterable
- so can use format
- for line in open(file.txt)
- bytearray can be used to store amorphous data via a constructor
- bytearray objects are muteable, like lists, and have length,
- bytearray - can only hold integers 0 - 255 inclusive
- bytearray can be written to files using binary
- a bytearray object can be passed to an open binary stream to read the data b.readinto(data)
- read() can also be used to read from binary file, this can then be passed to new bytearray 
- note - ideally limit or check data before using read() as it reads a whole file into memory, eg limit by size, buffer etc
- but arguments can be passed to read() to specify the max number of bytes read, 
-



