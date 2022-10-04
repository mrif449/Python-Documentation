# Chapter-2: Branching
[Back to main menu](../../README.md)
## <u>**Boolean Expression:**</u> 
In boolean expression we compare two values or two statements using the comparison operator to get the Boolean value (True/False).

1. <u>Comparison Operator:</u> We have 6 types of comparison or relational operators.

    1. Equal (==) : Returns True if the given two statements or values are True. Else, returns False.
    **Note:** Single equal (=) is used for value assignment, and Double equal (==) is used for equality checker comparison operator.
    2. Less than (<) : If the first statement or value is less than the second value than it returns True. Else, returns False.
    3. Greater than (>): If the first statement or value is greater than the second value than it returns True. Else, returns False.
    4. Less than Equal (<=): If the first statement or value is less  or equal than the second value than it returns True. Else, returns False.
    5. Greater than Equal (>=): If the first statement or value is greater  or equal than the second value than it returns True. Else, returns False.
    6. Not Equal (!=): If the two statements or values are not equal then it returns True. Else, returns False.

    **Example:**
    <img src="./images/19. comparison operator.png" width="100%"/>
2. <u>Logical Operator:</u> We have 3 types of Logical operators.

    1. and (Logical AND): The logical and returns True if all the statements are True. Else, returns False.
    2. or (Logical OR): The logical or returns True if any one of the statements are True. Else, returns False.
    3. not (Logical Not): Returns True, if False is given and vise versa.
    
    <img src="./images/20. note logical operator.png" width="100%"/>

    **Example:**
    <img src="./images/21. logical operator.png" width="100%"/>

### <u>Compound Boolean Expression:</u>
In this expression both logical and comparison operators are used together.

**Example:**
<img src="./images/22. compund logical expression.png" width="100%"/>

### <u>Conditional Statements:</u>
Comparison operators are basically used for writing conditional statements. They have 3 parts:
1. a condition yielding in either True or False.
2. a block of code is executed if the condition yields True.
3. another non-mandatory block of code is executed if the condition yields False.

    **Flowchart:**

    <p align=center><img src="./images/23. conditonal statement flowchart.png" width="40%"/></p>

### <u>Indentation:</u>
Indentation means leading whitespace (spaces and tabs) at the beginning of a particular line of code. It is basically used for grouping a section of code. A particular section or bundle of code is called “Block”. For example, in the previous flowchart, “True block” holds a section of code, which will only be executed if the condition yields True and “False block” holds a section of code, which will only be executed if the condition yields False. So, for blocking or in more general terms for paragraphing one or multiple lines, we use indentations.

1. <u>Basic Conditional Statement:</u>
    
    **Code Structure:**
    ```
        if (condition):
            #codes inside True block
            True block
            #codes inside True block
        else:
            #codes inside False block
            False block
            #codes inside False block
        #codes outside False block
    ```
    **Example:**

    <img src="./images/24. basic conditional statement.png" width="100%">

2. <u>Unary Selection (Omitting the else Clause):</u> When the condition evaluates to True, the True block is executed and the else and False block is completely excluded.
    
    **Code Structure:**
    ```
    if(condition):
        #codes inside True block
        True block
        #codes inside True block
    #codes outside True block
    ```
    **Flowchart:**
    
    <p align = center ><img src="./images/25. unary selection flowchart.png" width="40%"/></p>

    **Example:**

    <img src="./images/26. unary selection.png" width="100%"/></p>

3. <u>Nested Conditions:</u> Multiple conditional statements including unary selection statements can be nested inside one another. These are called nested conditional statements. Any number of these statements can be nested inside one another. Indentation is the only way to figure out the level of nesting. Here in the
flowchart below, we can see that inside the True block and False block, there is another set of conditions with True block and False block. There True block and False block again can have conditions nested inside them.

    **Flowchart:**
    
    <p align = center ><img src="./images/27. nested condition flowchart.png" width="65%"/></p>

    **Code Structure:**
    ```
    if (condition):
        #codes inside True block
        if (condition):
            #codes inside True block
            if (condition):
                True block
            else:
                False block
            #codes inside False block
        else:
            False block
        #codes inside False block
        if (condition):
            True block
        else:
            False block
        #codes inside False block
    #codes outside False block
    ```
4. <u>Chained or Ladder Condition:</u> The same checking of “nested conditionals” can be done using Chained conditionals (if….elif….elif….else). The conditions are checked from top to bottom. First the “if condition” is checked, if it yields False, then the next “elif condition” is checked. One if block, can have multiple “elif blocks” and only one “else block” at the end of the ladder, which is executed if the rest of the conditions yield False. The full form of “elif” is “else if”. Among several conditions of if...elif...else blocks, only one block is executed according to the condition.

    **Flowchart:**
    <p align = center ><img src="./images/28. chained condition flowchart.png" width="60%"/></p>

    **Code Structure:**
    ```
    if (condition):
        #codes inside if block
        if code block
        #codes inside if block
    elif (condition):
        #codes inside elif block
        elif code block
        #codes inside elif block
    elif (condition):
        #codes inside elif block
        elif code block
        #codes inside elif block
    else:
        #codes inside else block
        else code block
        #codes inside else block
    #codes outside if-elif-else block
    ```
[Back to main menu](../../README.md)