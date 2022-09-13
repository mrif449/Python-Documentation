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
    
    **Dictionary:** Dictionary. Dictionaries are used to store data values in key:value pairs. A dictionary is a collection which is ordered*, changeable and do not allow duplicates.

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
<img align=center src="./images/print statement.png" width="100%"/>

2. **Datatype Cheking:** Python uses a built is function "type()" to check what type of data is provided inside the function.
```
print(type("Python is easier than C++"))
```
```
print(type(1991))
```

<img align=center src="./images/type function.png" width="100%"/>

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
<img align=center src="./images/reserved keyword.png" width="100%"/>

### **<u>Operators</u>**
1. **Unary operations:** 
    1. <u>Unary +(plus):</u> We use unary + (plus) operation by adding a ‘+’ before a variable or data. It does not change the data. (Works with int, float, complex, and boolean. For booleans, True and False will be valued as 1 and 0 respectively.)

    **Example:**
    <img align=center src="./images/unary plus.png" width="100%"/>

    2. <u>Unary -(minus):</u> We use unary - (minus) operation by adding a ‘-’ before a variable or data. It produces the negative value of the input (equivalent to the multiplication with - 1). (Works with int, float, complex, and boolean. For booleans, True and False will be valued as 1 and 0 respectively.)

    **Example:**
    <img align=center src="./images/unary minus.png" width="100%"/>

    3. <u>Unary ~ (invert):</u> We use unary - (invert) operation by adding a ‘~’ before a variable or data. It produces a bitwise inverse of a given data. Simply, for any data x, a bitwise inverse is defined in python as -(x+1). (Works with int, and boolean. For booleans, True and False will be valued as 1 and 0 respectively.)

    **Example:**
    <img align=center src="./images/unary invert.png" width="100%"/>
2. **Binary operations:** Operators are symbols that represent any kind of computation such as addition, subtraction,
and etc. The values or the variables the operator works on are called Operands.(1+2) Where, 1 and 2 are operands, and + is the operator computing addition.
    1. <u>Arithmetic operation:</u> The arithmetic operations are: (+) Addition, (-) Subtraction, (*) Multiplication, (/) Division, (//) Floor Division, (%) Modulus.

    **Example:**
    <img align=center src="./images/arithmetic operation.png" width="100%"/>

    <img align=center src="./images/other arithmatic operation.png" width="100%"/>
    
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
        <img align=center src="./images/compound assignment operator.png" width="100%"/>

    3. <u>Logical Operator:</u> These operators mainly used on conditions, loops and many other places.
        1. and (Logical AND): If all the statements are True, then the operation will be executed.
        2. or (Logical OR): If one of the statements are True, then the operation will be executed.
        3. not (Logical NOT): If the statement is not True, then the operation will be executed.
         
        **Note:** More details will be discussed on Branching.
    4. <u>Membership Operator:</u> Returns Boolean as output. It is used as condition.
        1. in: Returns True, if the value is present on elements. Otherwise, returns False.
        2. not in: Returns True, if the value is **not** present on elements. Otherwise, returns False.

        **Example:**
        <img align=center src="./images/membership operator.png" width="100%"/>
    5. <u>Identity Operators:</u> These operators also returns boolean like Membership oprators.
        1. is: Returns True if the first value is identical or the same as the second value. Otherwise, returns False.
        2. is not: Returns True if the first value is **not** identical or the same as the second value. Otherwise returns False.

        **Example:**
        <img align=center src="./images/identity operator.png" width="100%"/>
    6. <u>Bitwise Operator:</u> Not used in basic coding. Will be discussed later(if necessary).
        1. & (Bitwise and)
        2. | (Bitwise or)
        3. ^ (Bitwise 1's complement)
        4. << (Bitwise left-shift)
        5. >> (Bitwise right-shift)