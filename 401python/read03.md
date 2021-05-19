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
                print(fnf_error)

- From the Shell:

        Doing something.
        [Errno 2] No such file or directory: 'file.log'



- Using finally - try, except, else, finally. The finally clause will still run despite hitting any execptions.

- adding to the code above from the article's example:

        finally:
            print('Cleaning up, irrespective of any exceptions.')











[code401 Reading Notes](/401Python/code401Table.md)