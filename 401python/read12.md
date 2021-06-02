# 10 minutes to Pandas

https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html

Dataframe - framing the data by passing a Numpy array to it. You can frame a list, dictonaries

from article:

Creating a DataFrame by passing a NumPy array, with a datetime index and labeled columns:

        In [5]: dates = pd.date_range("20130101", periods=6)

        In [6]: dates
        Out[6]: 
        DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
                    '2013-01-05', '2013-01-06'],
                    dtype='datetime64[ns]', freq='D')

        In [7]: df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list("ABCD"))

        In [8]: df
        Out[8]: 
                        A         B         C         D
        2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
        2013-01-02  1.212112 -0.173215  0.119209 -1.044236
        2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
        2013-01-04  0.721555 -0.706771 -1.039575  0.271860
        2013-01-05 -0.424972  0.567020  0.276232 -1.087401
        2013-01-06 -0.673690  0.113648 -1.478427  0.524988
Creating a DataFrame by passing a dict of objects that can be converted to series-like.

        In [9]: df2 = pd.DataFrame(
        ...:     {
        ...:         "A": 1.0,
        ...:         "B": pd.Timestamp("20130102"),
        ...:         "C": pd.Series(1, index=list(range(4)), dtype="float32"),
        ...:         "D": np.array([3] * 4, dtype="int32"),
        ...:         "E": pd.Categorical(["test", "train", "test", "train"]),
        ...:         "F": "foo",
        ...:     }
        ...: )
        ...: 

        In [10]: df2
        Out[10]: 
            A          B    C  D      E    F
        0  1.0 2013-01-02  1.0  3   test  foo
        1  1.0 2013-01-02  1.0  3  train  foo
        2  1.0 2013-01-02  1.0  3   test  foo
        3  1.0 2013-01-02  1.0  3  train  foo

- You can check the data type using dtype

# Viewing data

from article: 
Here is how to view the top and bottom rows of the frame:

        In [13]: df.head()
        Out[13]: 
                        A         B         C         D
        2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
        2013-01-02  1.212112 -0.173215  0.119209 -1.044236
        2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
        2013-01-04  0.721555 -0.706771 -1.039575  0.271860
        2013-01-05 -0.424972  0.567020  0.276232 -1.087401

        In [14]: df.tail(3)
        Out[14]: 
                        A         B         C         D
        2013-01-04  0.721555 -0.706771 -1.039575  0.271860
        2013-01-05 -0.424972  0.567020  0.276232 -1.087401
        2013-01-06 -0.673690  0.113648 -1.478427  0.524988
        Display the index, columns:

        In [15]: df.index
        Out[15]: 
        DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
                    '2013-01-05', '2013-01-06'],
                    dtype='datetime64[ns]', freq='D')

        In [16]: df.columns
        Out[16]: Index(['A', 'B', 'C', 'D'], dtype='object')

> "DataFrame.to_numpy() gives a NumPy representation of the underlying data. **NumPy arrays have one dtype for the entire array, while pandas DataFrames have one dtype per column.** When you call DataFrame.to_numpy(), pandas will find the NumPy dtype that can hold all of the dtypes in the DataFrame. This may end up being object, which requires casting every value to a Python object."


> "describe() shows a quick statistic summary of your data:"

> "Using the isin() method for filtering"

> "Concatenating pandas objects together with concat():"

# Grouping

> "By “group by” we are referring to a process involving one or more of the following steps:
> 1. Splitting the data into groups based on some criteria
> 2. Applying a function to each group independently
> 3. Combining the results into a data structure"

From article:

> "The stack() method “compresses” a level in the DataFrame’s columns."

        In [96]: stacked = df2.stack()

        In [97]: stacked
        Out[97]: 
        first  second   
        bar    one     A   -0.727965
                    B   -0.589346
            two     A    0.339969
                    B   -0.693205
        baz    one     A   -0.339355
                    B    0.593616
            two     A    0.884345
                    B    1.591431
        dtype: float64

> "With a “stacked” DataFrame or Series (having a MultiIndex as the index), the inverse operation of stack() is unstack(), which by default unstacks the last level:"

        In [98]: stacked.unstack()
        Out[98]: 
                            A         B
        first second                    
        bar   one    -0.727965 -0.589346
            two     0.339969 -0.693205
        baz   one    -0.339355  0.593616
            two     0.884345  1.591431

        In [99]: stacked.unstack(1)
        Out[99]: 
        second        one       two
        first                      
        bar   A -0.727965  0.339969
            B -0.589346 -0.693205
        baz   A -0.339355  0.884345
            B  0.593616  1.591431

        In [100]: stacked.unstack(0)
        Out[100]: 
        first          bar       baz
        second                      
        one    A -0.727965 -0.339355
            B -0.589346  0.593616
        two    A  0.339969  0.884345
            B -0.693205  1.591431

[code401 Reading Notes](../401Python/code401Table.md)