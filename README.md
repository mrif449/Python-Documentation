# Python Documentation
## List of Chapters
<details>
<summary>Basic</summary>

1. Data types, Values, Variables and Operators

2. Branching

3. Iteration

4. String Functions

5. Data Structure I (String, List, Tuple)

6. Data Structure II (Dictionary)

7. Function

8. Scope

9. File IO

</details>
<details>
<summary>Object Oriented Programming (OOP)</summary>
</details>
<details>
<summary>Data Structure</summary>
</details>
<details>
<summary>Algorithm</summary>
</details>


## Chapter-1: Data types, Values, Variables and Operators
### **<u>Data types</u>**
1. <u>**Numeric:** </u>
    1. **Integer** (int): Positive or negative whole numbers without any fractional part.
    **Example:** 1,2,3,-4,-22
    2. **Floating Point** (float): Any real numbers with “decimal” points or floating-point representation.
2. <u>**Boolean (bool):**</u> It represents only True and False.
3. <u>**Sequence:**</u> A sequence is an ordered collection of similar or different data types.
    1. **String (str):** It is a sequence if ordered characters including alphabets(uppercase, lowercase, numeric and special symbols)
        
        Example: “ABC”, “String123”, “hello112!!”
        
        **Note:** String is written with “” / ‘’ in python. Single of Double any quotation mark can be used.
        
    2. **List (list):** This is a ordered collections of elements which are separated with comma(,) and enclosed with square brackets[]. Any type of data can be stored in the list.
        
        **Example:**

        ```
        fruits = [”mango”,”berry”,”water melon”]
        ```
        ```
        things = [[”coding”,”programming”],[”Python”,”C++”],123,None]
        ```
        
        **Note:** One list can have more than one data type inside it. A list can be stored inside another list, which is called nested list.
        
    3. **Tuple** : Tuples are used to store multiple items in a single variable. Tuple is one of 4 built-in data types in Python used to store collections of data. Parenthesis() is used to indicate the Tuple.
        
        **Example:** 
        ```
        fruits = (”mango”,”berry”,”water melon”) things = ((”coding”,”programming”),(”Python”,”C++”),123,None)
        ```

        **Note:** One tuple can have more than one data type inside it. A tuple can be stored inside another list, which is called nested tuple. More will be discussed later
4. <u>**Mapping:**</u>
    
    **Dictionary:** Dictionaries are used to store data values in key:value pairs. A dictionary is a collection which is ordered*, changeable and do not allow duplicates.

    ```
    thisdict = {"Language": "Python","Founder": "Guido van Rossum","year": 1991}
    ```
5. **NoneType: (None):** It refers to a null value or no value at all. It's a special data type with a
single value, None.

### <u>**Some Extra Tips:**</u>

1. **Print any statement:** Python uses a built is function "python()" to show any output.

<u>Example:</u>

```
print("Rahadul Islam")
```
```
print(123)
```
<img src="./images/1. print statement.png" width="100%"/>

2. **Datatype Cheking:** Python uses a built is function "type()" to check what type of data is provided inside the function.
```
print(type("Python is easier than C++"))
```
```
print(type(1991))
```
<img src="./images/2. type function.png" width="100%"/>

3. **Take any Input:** Python uses a built is function "python()" to show any output. We basically take 3 types of input in python.

    1. <u>String:</u> To take string as input in Python, we can directly use input() funciton.
        
        **Example:**
        ```
        name = input("Enter a Progamming Language Name: ")
        print(name)
        ```
        <img src="./images/3. input str.png" width="100%"/>
    
    2. <u>Integer:</u> To take integer as input in Python, we use input() funciton and then we put that input function inside another built in function int().

        **Example:**
        ```
        year = int(input("Enter your birth year: "))
        print(name)
        ```
        <img src="./images/4. input int.png" width="100%"/>
    3. <u>Float:</u> To take float as input in Python, we use input() funciton and then we put that input function inside another built in function float().

        **Example:**
        ```
        marks = float(input("Enter your marks: "))
        print(marks)
        ```
        <img src="./images/5. input float.png" width="100%"/>

### **<u>Variable</u>**
A variable is a symbolic name that stores any type of data in Python. After assigning a variable to the data, that data can be called or used by the variable name.

**Example:** Here we want to store my name in a variable called "name" and print my name. The code will be:

```
name = "Md. Rahadul Islam Fardin"
print(name)
```
Here the "name" is the variable and "Md. Rahadul Islam Fardin" is the value of the variable.

**Variable Naming Conventions:**
1. Variable can have any letters(A-Z and a-z), digits(0-9) and underscores(_).
2. Variable can not start with digits.
3. Variable name should maintain snake_casing. That means, each word is separated by underscores(_).
4. Python is case-sensitive language. That means, "Name" and "name" are different variables.
5. Variable name should not be too lengthy or too short. Minimum length should be 3.
6. Variable name can not be any reserved keyword for Python. (<u>Example:</u> and, for, or, while).
7. Variable name can not have whitespace and special signs (<u>Example:</u> +, -, !, @, $, #, %.).

### Python Reserved Keywords:
<img src="./images/6. reserved keyword.png" width="100%"/>

### **<u>Operators</u>**
1. **Unary operations:** 
    1. <u>Unary +(plus):</u> We use unary + (plus) operation by adding a ‘+’ before a variable or data. It does not change the data. (Works with int, float, complex, and boolean. For booleans, True and False will be valued as 1 and 0 respectively.)

    **Example:**
    <img src="./images/7. unary plus.png" width="100%"/>

    2. <u>Unary -(minus):</u> We use unary - (minus) operation by adding a ‘-’ before a variable or data. It produces the negative value of the input (equivalent to the multiplication with - 1). (Works with int, float, complex, and boolean. For booleans, True and False will be valued as 1 and 0 respectively.)

    **Example:**
    <img src="./images/8. unary minus.png" width="100%"/>

    3. <u>Unary ~ (invert):</u> We use unary - (invert) operation by adding a ‘~’ before a variable or data. It produces a bitwise inverse of a given data. Simply, for any data x, a bitwise inverse is defined in python as -(x+1). (Works with int, and boolean. For booleans, True and False will be valued as 1 and 0 respectively.)

    **Example:**
    <img src="./images/9. unary invert.png" width="100%"/>
2. **Binary operations:** Operators are symbols that represent any kind of computation such as addition, subtraction,
and etc. The values or the variables the operator works on are called Operands.(1+2) Where, 1 and 2 are operands, and + is the operator computing addition.
    1. <u>Arithmetic operation:</u> The arithmetic operations are: (+) Addition, (-) Subtraction, (*) Multiplication, (/) Division, (//) Floor Division, (%) Modulus.

    **Example:**
    <img src="./images/10. arithmetic operation.png" width="100%"/>

    <img src="./images/11. other arithmatic operation.png" width="100%"/>
    
    2. <u>Assignment Operator:</u>
        
        1. =(assign): It is used for putting value from the right side of the equal sign(=) to a variable on the left side of the equal sign(=).

        **Example:** ``` number = 123```
        
        2. Compound Assignment Operators:
            
            1. += (add & assign)
            2. -= (subtract & assign)
            3. *= (multiply & assign)
            4. /= (divide & assign)
            5. %= (modulus & assign)
            6. **= (exponent & assign)
            7. //= (floor division & assign)

        **Example:**
        <img src="./images/12. compound assignment operator.png" width="100%"/>

    3. <u>Logical Operator:</u> These operators mainly used on conditions, loops and many other places.
        1. and (Logical AND): If all the statements are True, then the operation will be executed.
        2. or (Logical OR): If one of the statements are True, then the operation will be executed.
        3. not (Logical NOT): If the statement is not True, then the operation will be executed.
         
        **Note:** More details will be discussed on Branching.
    4. <u>Membership Operator:</u> Returns Boolean as output. It is used as condition.
        1. in: Returns True, if the value is present on elements. Otherwise, returns False.
        2. not in: Returns True, if the value is **not** present on elements. Otherwise, returns False.

        **Example:**
        <img src="./images/13. membership operator.png" width="100%"/>
    5. <u>Identity Operators:</u> These operators also returns boolean like Membership oprators.
        1. is: Returns True if the first value is identical or the same as the second value. Otherwise, returns False.
        2. is not: Returns True if the first value is **not** identical or the same as the second value. Otherwise returns False.

        **Example:**
        <img src="./images/14. identity operator.png" width="100%"/>
    6. <u>Bitwise Operator:</u> Not used in basic coding. Will be discussed later(if necessary).
        1. "&" (Bitwise and)
        2. "|" (Bitwise or)
        3. "^" (Bitwise 1's complement)
        4. "<<" (Bitwise left-shift)
        5. ">>" (Bitwise right-shift)

### <u>**Type Conversion:**</u> Datatypes can be modified in 2 ways.
1. <u>Implicit Type Conversion:</u> If any of the operands are floating-point, then arithmetic operation yields a floating- point value. If the result was integer instead of floating-point, then removal of the fractional part would lead to the loss of information.

    **Example:** 
    <img  src="./images/15. implicit type conversion.png" width="100%"/>

2. <u>Explicit Type Conversion:</u> Conversion among different data types are possible by using type conversion functions, though there are few restrictions. Python has several functions for this purpose among them these 3 are most used:
    
    1. <u>String -> str():</u> It constructs a string from various data types such as strings, integer numbers and float-point numbers.

        **Example:**
        <img src="./images/16. explicit type conversion str.png" width="100%"/>
    2. <u>Integer -> int():</u> constructs an integer number from various data types such as strings ( the input string has to consist of numbers without any decimal points, basically whole numbers), and float-point numbers (by rounding up to a whole number, basically it truncates the decimal part).
        **Example:**
        <img src="./images/17. explicit type conversion int.png" width="100%"/>
    3. <u>Float -> float():</u> This constructs a floating-point number from various data types such as integer numbers, and strings (the input string has to be a whole number or a floating point number).
        **Example:**
        <img src="./images/18. explicit type conversion float.png" width="100%"/>

## Chapter-2: Branching

### <u>**Boolean Expression:**</u> 
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