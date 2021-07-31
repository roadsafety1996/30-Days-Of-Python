
## Classes and Objects

Python is an object oriented programming language. Everything in Python is an object, with its properties and methods. A number, string, list, dictionary, tuple, set etc. used in a program is an object of a corresponding built-in class. We create class to create an object. A class is like an object constructor, or a "blueprint" for creating objects. We instantiate a class to create an object. The class defines attributes and the behavior of the object, while the object, on the other hand, represents the class.

>>> num = 10
>>> type(num)
<class 'int'>
>>> string = 'string'
>>> type(string)
<class 'str'>
>>> boolean = True
>>> type(boolean)
<class 'bool'>
>>> lst = []
>>> type(lst)
<class 'list'>

### Creating a Class

To create a class we need the key word **class** followed by the name and colon. Class name should be **CamelCase**.

```sh
# syntax
class ClassName:
  code goes here
```
**Example:**
```py
class Person:
  pass
print(Person)
```sh
<__main__.Person object at 0x10804e510>
```
### Creating an Object

We can create an object by calling the class.

```py
p = Person()
print(p)
