# Comparison Operators
This compares one value to what the expectation is, this results in a Boolean; true or false.

- == - "is equal to" - This particular operator compares 2 values and sees if they are the same. (These values are either number Booleans, or strings)

        -'Yes' == 'No' returns false
        -'Yes' == 'Yes' return true

- != - "is not equal to" - The particular operator compares 2 values and sees if they aren't the same. (These values are either number Booleans, or strings)

        -'Yes' != 'No' returns true
        -'Yes' != 'Yes' returns false


- === - "strict equal to" - This particular operator compares 2 values and sees if both the data type and value are the same.

        -'16' === 16 returns false
        -'16' === '16' returns true

- !=== - 'strict not equal to' - Will compare 2 values and determine if both data type and value are **not** the same.

        -'16' !== 16 returns true
        -'16' !== '16' returns false

- > - "greater than" - Will determine if number on left is greater than number on right.

        - 16 > 5 returns true
        - 16 > 24 returns false

- < - "less than' - Will determine if number on left is is less than number on right.

        - 16 > 5 returns false
        - 16 > 24 returns true

- >= - "greater than or equal to" - Will determine if number on left is greater than or equal to number on right. 

        16 >= 5 returns true 
        16 >= 24 returns false
        16 >= 16 returns true

- <= - "greater than of equal to" - Will determin if number on left is less than or equal to number on right.

        16 <= 5 returns false
        16 <= 24 returns true
        16 <= 16 returns true

# Logical Operators

- && - Logical And - tests more than only one condition within an expression. 

        ((3 < 7) && (4 >=1))
        return is true

If both of our expression come back as true, then the expression returns to us as true. If there is just one of the expressions above return as false, then it will return as false. Both must be true.

- || - Locical OR - test at least on of the conditions below. 

        ((3 < 7) || (4 < 1))

If only one of the expressions above come back, return, as true, then the expression returns true. If both of the expressions return as false, then the expression will be false. At least one has to be true, both have to be false in order for it to be false.

- ! - Logical Not - This inverts a the value of single Boolean. 

        !(3 < 7)
        returns false

The logical not flips our expression state to the opposite. 


# Loops
    
- for - running code for a specific number of times, like an incorrect password. This one is a counter, meaning it will count your incorrect answers. This will be told by the condition how many times the loop should run. 

- while - a loop where you have no idea how many times it should run. This loop will continue until the condition is met and returns true. 

- do while - the do while loop, closely resembling the while loop, has one difference. it will run statements at a minimum of at least once even if it returncomes backs false.

# Loop Counters

**Statements within the for loop**

- Initialization - we set our variable to 0. Our variable is called i. and it behave as our counter. This is our starting position. Starts at 0.

        ver i = 0;

- Condition - the for loop will run until it hits outour specified number. If we start at 0, the loop will run 5 times, 0, 1, 2 ,3 ,4 ,5, undefined.

        i < 5;

- Update - we add one to our counter after each time the loop runs.

        i++

SO;

        let i;
        for (i = 0; i < 10; i++){
                "code"
        }


[Back to Homepage](README.md)