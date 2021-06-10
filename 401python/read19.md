# Python Regular Expression Tutorial
https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial

> "The match() function returns a match object if the text matches the pattern."

> "Do you notice the r at the start of the pattern Cookie? This is called a raw string literal. It changes how the string literal is interpreted. Such literals are stored as they appear. For example, \ is just a backslash when prefixed with an r rather than being interpreted as an escape sequence. You will see what this means with special characters. Sometimes, the syntax involves backslash-escaped characters, and to prevent these characters from being interpreted as escape sequences; you use the raw r prefix."

> ". - A period. Matches any single character except the newline character."

> "^ - A caret. Matches the start of the string. This is helpful if you want to make sure a document/sentence starts with certain characters."

>"$ - Matches the end of string. This is helpful if you want to make sure a document/sentence ends with certain characters."

> "\ - Backslash.
Perhaps, the most diverse metacharacter!! If the character following the backslash is a recognized escape character, then the special meaning of the term is taken (Scenario 1) Else if the character following the \ is not a recognized escape character, then the \ is treated like any other character and passed through (Scenario 2). \ can be used in front of all the metacharacters to remove their special meaning (Scenario 3)."

> "compile(pattern, flags=0)" - caches expressions. Regular expressions are handled as strings by Python. However, with compile(), you can computer a regular expression pattern into a regular expression object. When you need to use an expression several times in a single program, using compile() to save the resulting regular expression object for reuse is more efficient than saving it as a string. This is because the compiled versions of the most recent patterns passed to compile() and the module-level matching functions are cached."

> "search(pattern, string, flags=0) - With this function, you scan through the given string/sequence, looking for the first location where the regular expression produces a match. It returns a corresponding match object if found, else returns None if no position in the string matches the pattern. Note that None is different from finding a zero-length match at some point in the string."

> "match(pattern, string, flags=0) - Returns a corresponding match object if zero or more characters at the beginning of string match the pattern. Else it returns None, if the string does not match the given pattern."
> "findall(pattern, string, flags=0) - Finds all the possible matches in the entire sequence and returns them as a list of strings. Each returned string represents one match."

> "finditer(string, [position, end_position]) - Similar to findall() - it finds all the possible matches in the entire sequence but returns regex match objects as an iterator."

> "sub(pattern, repl, string, count=0, flags=0) - sub() is the substitute function. It returns the string obtained by replacing or substituting the leftmost non-overlapping occurrences of pattern in string by the replacement repl. If the pattern is not found, then the string is returned unchanged."

> "subn(pattern, repl, string, count=0) - The subn() is similar to sub(). However, it returns a tuple containing the new string value and the number of replacements that were performed in the statement."

# shutil — High-level File Operations

https://pymotw.com/3/shutil/

# Youtube - Super Quick Python Automation Ideas

https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s


# Al Sweigart, "Automating Your Browser and Desktop Apps", PyBay2016

https://www.youtube.com/watch?v=dZLyfbSQPXI


# Watchdog

https://pythonhosted.org/watchdog/

# Regular Expressions in Python - FULL COURSE (1 HOUR) - Programming Tutorial
https://www.youtube.com/watch?v=AEE9ecgLgdQ


[code401 Reading Notes](../401Python/code401Table.md)