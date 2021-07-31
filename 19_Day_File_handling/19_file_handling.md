

## File Handling

So far we have seen different Python data types. We usually store our data in different file formats. In addition to handling files, we will also see different file formats(.txt, .json, .xml, .csv, .tsv, .excel) in this section. First, let us get familiar with handling files with common file format(.txt).

File handling is an import part of programming which allows us to create, read, update and delete files. In Python to handle data we use _open()_ built-in function.

```py
# Syntax
open('filename', mode) # mode(r, a, w, x, t,b)  could be to read, write, update
```

- "r" - Read - Default value. Opens a file for reading, it returns an error if the file does not exist
- "a" - Append - Opens a file for appending, creates the file if it does not exist
- "w" - Write - Opens a file for writing, creates the file if it does not exist
- "x" - Create - Creates the specified file, returns an error if the file exists
- "t" - Text - Default value. Text mode
- "b" - Binary - Binary mode (e.g. images)

### Opening Files for Reading

The default mode of _open_ is reading, so we do not have to specify 'r' or 'rt'. I have created and saved a file named reading_file_example.txt in the files directory. Let us see how it is done:
```py
f = open('./files/reading_file_example.txt')
print(f) # <_io.TextIOWrapper name='./files/reading_file_example.txt' mode='r' encoding='UTF-8'>
```

As you can see in the example above, I printed the opened file and it gave  some information about it. Opened file has different reading methods: _read()_, _readline_, _readlines_. An opened file has to be closed with _close()_ method.

- _read()_: read the whole text as string. If we want to limit the number of characters we want to read, we can limit it by passing int value to the *read(number)* method.

```py
f = open('./files/reading_file_example.txt')
txt = f.read()
print(type(txt))
print(txt)
f.close()
```
```sh
# output
<class 'str'>
This is an example to show how to open a file and read.
This is the second line of the text.
```
