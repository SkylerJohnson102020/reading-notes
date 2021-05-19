# Python Exceptions: An Introduction

https://realpython.com/python-exceptions/

- Python terminates once it hits an error, but there are exceptions.

- An exception is different from a syntax error. It is when python code that is correct hits an error. The error will be detailed. The code is syntactically correct, but the statements are not. In the example, 0 divided by 0 threw the error.

- Raise can be used to force an exception. Example below from article:

        x = 10
        if x > 5:
            raise Exception('x should not exceed 5. The value of x was: {}'.format(x))

- When the code is run, it stops and the error from the raise is shown with the data injected into the exception.

- AssertionError Exception - You set, or assert, that a condition is met. You are good to go if the assertion turns True. If False, the program can throw an Assertion Error. The AssertionError is the final thing that the program will execute.

- try and except - used to catch and deal with exception handling. The code will run until it hits an exception. It can also inform you that some specific code did not run.

- Three takeaways quoted directly from the article:

> 1. A try clause is executed up until the point where the first exception is encountered.
> 2. Inside the except clause, or the exception handler, you determine how the program responds to the exception.
> 3. You can anticipate multiple exceptions and differentiate how the program should respond to them.

- The else clause (try, except, else) - The else clause allows you to run some code when no exceptions have been hit. You have the ability to set another try/except inside the else. Excellent example taken diretly from the article:

        try:
            linux_interaction()
        except AssertionError as error:
            print(error)
        else:
            try:
                with open('file.log') as file:
                    read_data = file.read()
            except FileNotFoundError as fnf_error:
                print(fnf_error
- From the Shell:

        Doing something.
        [Errno 2] No such file or directory: 'file.log'



- Using finally - try, except, else, finally. The finally clause will still run despite hitting any execptions.

- adding to the code above from the article's example:

        finally:
            print('Cleaning up, irrespective of any exceptions.')


# Read and Write Files in Python

https://realpython.com/read-write-files-python/

- A file is a collection of bytes used in storing some data. This data is then formatted to a file type. Three parts to a file for most files: Header, Data, End of File(EOF)

- Files Paths in three main parts - Folder Path, File Name, Extension.

- Problems one might encounter - Windows vs. Unix systems, Character Encodings.

- UTF-8 (Unicode) uses up to 1,114,112 characters.

- ASCII - a data encoding system which uses 128 characters, a subset of Unicode. This means Unicode and ASCII can share char values.

**PROBLEM** You can parse ASCII (128 char) to Unicode (1 mil plus), but not the opposite if a char falls outside of ASCII.

- Opening a file - use open() built-in method. One required arg, the file path.

- Closing a file - use close(). 2 ways to make sure you close a file properly.

    1. try finally (Example directly from the article below)
        
            reader = open('dog_breeds.txt')
            try:
                # Further file processing goes here
            finally:
                reader.close()

    2. with statement (Example directly from the article below). with automatically closes the file after it leaves the code block.
        
            with open('dog_breeds.txt') as reader:
            # Further file processing goes here

- A second arg passed into the with statement is a string to represnt how you want to open the file. Most commonly "r", for read-only.

            with open('dog_breeds.txt', 'r') as reader:
            # Further file processing goes here

- Also: "r" for read, "w" for open for writing/overwriting the file, "rb" or "wb" for open in binary mode.

- 3 categories of file objs
    1. text 
        - opening a file will return a TextioWrapper. The default onj returned.

    2. Buffered binary
        - type used to read and write binary files.
        - open() file returns BufferedReader or Buffered Writer file obj.

    3. Raw binary
        - not typically used since it's more of a raw building block. lower level.
        - open() return FileIO

- Read methods:
    .read(size) - is no arg, None, or -1 is passed in, entire file read.
    .readline(size) - same as above, only this reads the size number you pass in as the num of char in a line, then puts on a new line. The line will wrap to the next if more than indicated size.
    .readlines() - reads file, returns as list.

- iterating over each line - .readline() or readlines() - see examples in article


- Write methods:
    .write(string) - writes string to file
    .writelines(seq) - writes sequence to file.

- Writing in byte strings - instead of "r" as second arg, use "rb".

- str2unix() - which will turn \r\n into \n line endings.

- dos2unix() - converts a string containing \r\n to \n.


- Appending to a file - adding something to the end of an already populated file, use the "a" as your second arg to append. In the example, adding a new dog breed.

- you can read one file and write in another at the same time.

- Use these when using a custom class since with can no longer be used.

-       __enter__() - use when invoking the with statement

-       __exit__() - use when exiting the statement code block.


[code401 Reading Notes](/401Python/code401Table.md)