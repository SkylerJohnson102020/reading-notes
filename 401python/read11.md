# NumPy Tutorial: Data Analysis with Python

https://www.dataquest.io/blog/numpy-tutorial-python/

NumPy is a data analysis package.

## Numpy 2-Dimensional Arrays

- 2 dimensional array - matrix - a list of lists

from article:
> "In a NumPy array, the number of dimensions is called the rank, and each dimension is called an axis. So the rows are the first axis, and the columns are the second axis."

- A NumPy array can be created by using a numpy.array().

> "One of the limitations of NumPy is that all the elements in an array have to be of the same type,....."

- check number of rows in a NumPy array using .shape().

        empty_array = np.zeros((3,4))

        empty_array

> "It’s useful to create an array with all zero elements in cases when you need an array of fixed size, but don’t have any values for it yet."


## Using NumPy To Read In Files

> "It’s possible to use NumPy to directly read csv or other files into arrays. We can do this using the numpy.genfromtxt function. We can use it to read in our initial data on red wines."

> "In the below code, we:

> 1. "Use the genfromtxt function to read in the winequality-red.csv file."

> 2. "Specify the keyword argument delimiter=";" so that the fields are parsed properly."

> 3. "Specify the keyword argument skip_header=1 so that the header row is skipped."

        wines = np.genfromtxt("winequality-red.csv", delimiter=";", skip_header=1)

- Use two indexes to access data, row first, column second. so: `wines[2,3]`

## Slicing

> "If we instead want to select the first three items from the fourth column, we can do it using a colon (:). A colon indicates that we want to select all the elements from the starting index up to but not including the ending index. This is also known as a slice: code from article"

        wines[0:3,3]
        array([ 1.9, 2.6, 2.3])

See article for more on slicing.


## Assigning Values To NumPy Arrays
> "We can also use indexing to assign values to certain elements in arrays. We can do this by assigning directly to the indexed value: code from article"

    wines[1,5] = 10

> "We can do the same for slices. To overwrite an entire column, we can do this:"

    wines[:,10] = 50

> "The above code overwrites all the values in the eleventh column with 50."

## 1-Dimensional NumPy Arrays

- Also known as a vector, only need one index to access data

- By only giving one arg into shape(), we specify 1-dimensional, 2 args is a matrix or 2-dimensional.

## N-Dimensional NumPy Arrays

> "One way to think of this is a list of lists of list."

From article:

    year_one = [
        [500,505,490],
        [810,450,678],
        [234,897,430],
        [560,1023,640]
    ]

> "We can retrieve the earnings from January by calling year_one[0][0]. If we want the results for a whole quarter, we can call year_one[0] or year_one[1]. We now have a 2-dimensional array, or matrix. But what if we now want to add the results from another year? We have to add a third dimension:"

    earnings = [
        [
            [500,505,490],
            [810,450,678],
            [234,897,430],
            [560,1023,640]
        ],
        [
            [600,605,490],
            [345,900,1000],
            [780,730,710],
            [670,540,324]
        ]
    ]

> "We can retrieve the earnings from January of the first year by calling `earnings[0][0][0].`" 

> "If we wanted to get the earnings for January of all years, we could do this:"

    earnings[:,0,0]
    array([500, 600])

## NumPy Data Types

you can find the data type by using `.dtype()`.

The different data types, from article:

> float — numeric floating point data.
> int — integer data.
> string — character data.
> object — Python objects.

They also end with a suffix showing you how much memory they need. `int32`, `float64`, etc.

You can use `.astype()` to change the data type.

You can change how much memory it takes by assigning it: `np.int32`, `numpy.int32`

## Broadcasting

> "Essentially, broadcasting involves a few steps:
>The last dimension of each array is compared.
>If the dimension lengths are equal, or one of the dimensions is of length 1, then we keep going.
>If the dimension lengths aren’t equal, and none of the dimensions have length 1, then there’s an error.
> Continue checking dimensions until the shortest array is out of dimensions."

## NumPy methods

sum()
mean()
std() standard deviation
min() find min val
max() find max val



[code401 Reading Notes](../401Python/code401Table.md)