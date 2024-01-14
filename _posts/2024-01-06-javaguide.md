---
title: My Java Guide
date: 2024-01-06 13:35:00 +0600
categories: [programing]
tags: [guides]     # TAG names should always be lowercase
---

## <font color="#99FF99">Introduction to Java</font>  

Java
: Java is a powerful and versatile programming language that has been widely used for over two decades. It's known for its portability, security, and object-oriented approach.  

### <font color="#99FF99">Key features of Java</font>
- General-Purpose Programming Language
- Easy to learn 
- Write Once, Run Anywhere (WORA)
- Object-Oriented
- Secure
- Platform Independent
- It's Free!  

### <font color="#99FF99">Characteristics of Java</font>
- Uses C/C++ basic syntax and basic data types - int, char, float, double, long, short, byte etc.
- Uses standard C/C++ control structures
- “Pure” OO(Object Oriented) language
- No stand alone functions -All code is part of a class
- No explicit pointers - uses references
- Uses garbage collection
- Java is strongly typed
- Java is normally compiled to a bytecode.
- Java bytecode is a machine language for an abstract 
machine
- Makes Java secure and Portable
- Each platform (or browser) that runs Java has a Java 
Virtual Machine (JVM) . The JVM executes Java bytecodes


## <font color="#99FF99">Requirments to code in Java?</font>
We need a few things to get started.  
- JDK (Java Development Kit)
- An IDE or a Code/Text Editor  

Yep, that's all you need. ✅  

For this guide I'll be using the [Intellij IDEA](https://www.jetbrains.com/idea/download/?section=windows) IDE by JetBrains. But you can use any IDE or Code/Text editor. Some notable ones are [Eclipse](https://www.eclipse.org/downloads/), [NetBeans](https://netbeans.apache.org/front/main/download/index.html) and [Visual Studio Code](https://code.visualstudio.com/).

Now let's write our first code in Java!  

## <font color="#99FF99">Writing our first code</font>
Whenever we learn a new programming language, it has become a tradition that we start our journey by printing "Hello world". We'll be doing exactly that right now.  

```java

public class HelloWorld {
    public static void main(String[] args) {
        System.out.print("Hello world");
    }
}
```

**Here's a breakdown of each part of the code:**

**1. `public class HelloWorld`**

- **`public`:** This keyword means the class is accessible from anywhere in your program. It's like opening the door to the class for other parts of your code to use it.
- **`class`:** This keyword declares a new class, which is a blueprint for creating objects. It's like a template for building things.
- **`HelloWorld`:** This is the name you've given to the class. It's like giving a name to the blueprint.

**2. `public static void main(String[] args)`**

- **`public`:** Same as before, this means the method is accessible from anywhere.
- **`static`:** This means you can call this method without creating an object of the `HelloWorld` class. It's like having a tool that you can use directly without needing to build a whole machine first.
- **`void`:** This means the method doesn't return any value. It just does its job and then finishes.
- **`main`:** This is the special method that Java looks for to start your program. It's like the ignition switch that gets things going. It's the same as you've seen in C.
- **`(String[] args)`:** This part allows you to pass arguments (extra information) to the program when you run it. It's like giving instructions to the program before it starts. **`String[]`** is basically the name of the pre-defined class here. And **`args`** is the name of the string. You can name it anything you want.

 > Variable names must start with a letter, underscore (_), or dollar sign ($). Can contain nothing except letters, digits, underscores, and dollar signs
 and it cannot be a reserved keyword.
{: .prompt-warning }  

**3. `System.out.print("Hello world");`**

- **`System.out.print`:** This part tells Java to print something to the console (the text window where you see the output). It's like using a loudspeaker to speak to the user.
- **`"Hello world"`:** This is the text that you want to print to the console. It's the message you're sending to the user.

**In essence:**

- You're creating a class named `HelloWorld` that acts as a blueprint for your program.
- Inside that class, you have a method named `main` that Java runs when the program starts.
- The `main` method simply prints the message "Hello world" to the console to show that the program ran successfully.

**Congratulations!** 🥳 You've wrote your first Java program!  


## <font color="#99FF99">Terms we need to be clear about</font>  

### <font color="#99FF99">Keyword</font>
A keyword is any one of the reserved words, that have a predefined meaning in Java.  


In Java syntax, **all code is case-sensitive**, and this includes keywords. As we'll soon see, an **int**, all in lowercase, is not the same as **Int**, with a capital **I**. Here, an **int**,(all in lowercase) is a keyword in Java.  

Here is a list of keywords in the Java programming language. You cannot use any of the following as identifiers in your programs. The keywords const and goto are reserved, even though they are not currently used. `true`, `false`, and `null` might seem like keywords, but they are actually literals; you cannot use them as identifiers in your programs.

| Keywords in Java |               |             |
|    -----------   | ------------- | ----------- |
| abstract         | synchronized  | return
| continue         | this          | short
| for              | protected     | transient
| new              | throw         | try
| switch           | public        | void
| assert           | throws        | volatile
| default	       | goto	       | package
| boolean	       | do	if	       | private
| break	           | double	       | implements	
| byte	           | else	       | import
| case	           | enum	       | instanceof		
| catch	           | extends	   | int
| char	           | final	       | interface
| class	           | finally	   | long
| const*	       | float	       | native	
| while            | super	       | strictfp
| static	

### <font color="#99FF99">Variables</font>
Variables are **a way to store information in our computer**.

Variables that we define in a program, can be accessed **by a name we give them**, and the computer does the hard work of figuring out where they get stored in the computer's **Random Access Memory(RAM)**.

To create a variable, first we need to know about **Data Types**.  

#### Data Type
There are lots of **different types of data, that we can define for our variables**. Collectively, these are known as data types.

As you may have guessed, **some data types are keywords** in Java.  When we get to the Object Oriented features of Java, you will see that we have a lot of flexibility for creating our own data types, but for now, we'll explore **primitive data types**, which are **built into the Java language**.  

#### Define a variable
Now that we've understood what Data Types are, we may create a variable. To define a variable:
1. We need to specify the **data type**
2. Then, give our variable a **name**
3. ***Optionally***, <font color="#FFCC99">add an <b>expression</b> to initialize the variable with a value.</font>

```java

int myFirstNumber = 5;
```
We have just declared a variable of type `int` named `myFirstNumber` and assigned value `5` to our variable.

> Note that, we can assign a value to a variable multiple times in Java, but it’s the declaration (which includes the data type) that cannot normally be done a second time for the same variable.
{: .prompt-info }  

### <font color="#99FF99">Operators</font>
Operator
: Java operators, or just operators, perform an operation (hence the term) on a variable or value.  

Addition(`+`), Subtraction(`-`), Division(`/`), and Multiplication(`*`) are four common ones that I feel sure you're familiar with, but there are lots more operators you will work with later on.  

### <font color="#99FF99">Expressions</font>
Expression
: The expression is the code segment that is on the right side of the equals sign in an assignment or declaration statement.  

This code can be a simple literal value, like the number 5, or it can be a complex mathematical equation using multiple literal values and mathematical operators.  

### <font color="#99FF99">String Literals</font>

Text specified in double-quotes is called "string literals".

> Double quotes `(" ")`are used for string literals and single quotes`(' ')`are used for character literals.
{: .prompt-info }  

### Class
A class is a building block for object-oriented programming, and allows us to **build custom data types**.   

Basically, a class is a type of custom data type. Like for example, <i>you can use multiple integers to make a sort of super data type, which we will class a class in java.</i> And Java comes with a whole library of helpful classes.

### Wrapper Class
Java uses the concept of a wrapper class, for all of its eight primitive data types.

A wrapper class provides simple operations, as well as some basic information about the primitive data type, which cannot be stored on the primitive itself. 

MIN_VALUE, and MAX_VALUE, are elements of this basic information, for the int data type.  

|Primitive|Wrapper Class|
|---------|-------------|
|byte     |Byte         |
|short    |Short        |
|char     |Character    |
|int      |Integer      |
|long     |Long         |
|float    |Float        |
|double   |Double       |
|boolean  |Boolean      |  

### Overflow and Underflow in Java
If you try and put a value larger than the maximum value into an int, you'll create something called an Overflow situation.  

And similarly, if you try to put a value smaller than the minimum value into an int, you cause an Underflow to occur.  

These situations are also known as **integer wraparounds**.
<br/>  
<font color = "#FFCC99">The maximum value, when it overflows, wraps around to the minimum value, and just continues processing without an error.

The minimum value, when it underflows, wraps around to the maximum value, and continues processing.</font>  

This is not usually behavior you really want, and as a developer, you need to be aware that this can happen, and choose the appropriate data type.  

#### When will we get an overflow? when will you get an error?
An integer wraparound event, either an overflow or underflow, can occur in Java when you are using expressions that are not a simple literal value. 

The Java compiler doesn't attempt to evaluate the expression to determine its value, so it DOES NOT give you an error.

*<font color = "#FFCC99">Now look at these example below carefully</font>*  

Here are two more examples that will compile, and result in an overflow.  The second example may be surprising.  Even though we are using numeric literals in the expression, the compiler still won't try to evaluate this expression, and the code will compile, resulting in an overflow condition.

```java
int thisWillCompile = (Integer.MAX_VALUE + 1);
int thisWillCompile = (2147483647 + 1);
```
**BUT** if you assign a numeric literal value to a data type that is outside of the range, the compiler DOES give you an error.

![Alt text](/assets/img/sample/image.png)


> You can use underscores (`_`) to improve integer readablity.  
*Example:* `int a = 2_147_483_647;`  
Which will give you `a ==> 2147483647`
{: .prompt-tip }

## <font color="#99FF99">Before we start</font>  

Before we start our journey of Java, it's crusial to know certain things about it. Below are the things we need to understand to code on Java.  

### <font color="#99FF99">Java Code is case sensitive</font>
Java code is case sensitive.  

**This includes not only keywords and language syntax, but variable names and data types as well.**  

`myFirstNumber` is not the same variable as `MyFirstNumber` with a capital M.  

**int** in lowercase, is not the same as **Int** with the first letter capitalized, or **INT**, all in uppercase, etc.  

**Keywords need to be in lowercase.**  

And **variables will always be exactly as you declare them, including capitalization.**  

<font color="#FFCC99"><i>Remember that, case matters in Java code!</i></font>  


### <font color="#99FF99">How to name a java source file?</font>
- All java source file should end with .java  
    - <font color="#FFCC99"><i>Example : </i></font>`Hello.java`  

- Each `.java` file can contain only **one public class**.

- The name of the file should be the name of the public class plus ".java"  
    - <font color="#FFCC99"><i>Example : </i></font>If the public class is `public class HelloWorld` (HelloWorld), then the file name should be `HelloWorld.java`  

> As convention, if the class name contains multiple words then capitalize the first letter of each word.  
<i>Example:</i> `HelloWorld.java`
{: .prompt-info }  

### <font color="#99FF99">Java's Primitive Types</font>

In Java, Primitive Types are the most basic data types.  

The **eight** primitive data types in Java are shown in the tables below, listed by the type of data stored for each:

| Whole Number | Real number (floating point or decimal)|
| ------------ | --------------------------------------|  
|byte          | float                                 |
|short         | double                                |
|int           |
|int           |
|long          | 

|Single Character| Boolean Value |
|----------------| ------------- |       
| char           | boolean       |  

Consider these types as the building blocks of data manipulation.  

<font color="#FFCC99">Remember that primitive data types are simply placeholders in memory for a value.
</font>


### A look at the premitive data types

#### Integer
There's a specified range of values allowed for the int, which is true for most data types.  

What this means is, that the allowable range of values is NOT infinite.

There's a defined minimum, and maximum value, for each numeric data type, meaning you can't assign a number bigger or smaller (outside of that range).

##### Finding out the range of integer type
If we want to view the minimum value and the maximum value of an integer type data respectively, we can run the following code:

```java
public class Main {
    public static void main(String[] args) {

        int minIntValue = Integer.MIN_VALUE;
        int maxIntValue = Integer.MAX_VALUE;

        System.out.println("Minimun value of int data type = " + minIntValue);
        System.out.println("Maximum value of int data type = " + maxIntValue);
    }
}
```

The outputs will be as below:
```java
Minimun value of int data type = -2147483648
Maximum value of int data type = 2147483647
```
As we can see, the integer data type can hold a value from the range of -2147483648 to 2147483647.

##### Using the `+` sign with System.out.ptint
The plus sign, +,  when used in `System.out.print` will print different data types together as a single line of text.  

In the example above:

We want to print a label, before a numeric integer value. Whatever follows the plus sign in `System.out.print` here, is converted to a String by Java, and concatenated to the String before it.  

This is perfectly valid syntax in Java.

**Challenge :**
Try to find the output of this code segment below:
```java
public class HelloWorld {
    public static void main(String[] args) {

        System.out.println("Integer value range (" + Integer.MIN_VALUE + " to " + Integer.MAX_VALUE + ")");
    }
}
```

The output should be : `Integer value range (-2147483648 to 2147483647)`  

#### When is `L` required?
A numeric literal that exceeds `Integer.MAX_VALUE` must use the `L` suffix.  

We cannot create a numeric literal in Java, that exceeds `Integer.MAX_VALUE`, without using the `L` suffix, we'll always get the error `integer number too large`.

- for whole numbers, the output is never in scientific notation. but for real/decimal numbers, we can print it as we like, by using scintific notation or how many decimal points.

#### Floating point number precision tip
In general, float and double are great for general floating point operations. 

But neither should be used when precise calculations are required – this is due to a limitation with how floating point numbers are stored, and not a Java problem as such.

Java has a class called `BigDecimal` that overcomes this. 

#### Char

##### Comparing the char to the String

|char|String|
|----|------|
| Holds one, and only, one character | Can hold multiple characters |
| Literal closed in Single Quotes    | Literal closed in Double Quotes |

A char occupies two bytes of memory, or 16 bits, and thus has a width of 16.

The reason it's not just a single byte, is that a char is stored as a 2 byte number, similar to the short.  

This number gets mapped to a single character by Java.  

- So, when you print a char, you will see the mapped character, and not the representative number.
- And you can use single quotes and a character literal to assign a value to a char, which is much simpler than looking up the representative number.  


- You need to put a `\` to use a unicode. Example: `char myChar = '\u0044';` which is the unicode for letter `D`.  


#### Boolean
A boolean value allows for two opposite choices, true or false, yes or no, one or zero.  

In Java terms, we've got a boolean primitive type, and it can be set to **two** values only, either `true` or `false`.  

The wrapper for boolean is Boolean with a capital B.  

##### Why would you start your boolean variable name with the prefix "is" ?
Developers will often use the word, **is**, as a prefix for a boolean variable name.

This creates a name that seems to ask a question, which makes reading the code more intuitive.  

But other prefixes can be just as valid.  

Here are some example boolean variable names, such as isMarried and hasChildren, that clearly define what condition is being tested:  

|Boolean Variable name examples|
|------------------------------|
|isCustomerOverTwentyOne|
|isEligibleForDiscount|
|hasValidLicense|
|isMarried|
|hasChildren|

### Java's built-in classes

- Wrappers (Boolean, Double, Character, etc.)
- BigDecimal
- String  

### String

#### What is a string?
A String is a class that contains a sequence of characters.  

The String can contain a large number of characters. Its technically only limited by the ammount of memory space or heap space in your computer, which turns out to be the value of `Integer.MAX_VALUE`.  

#### String Concatenation
In Java, the `+` symbol is an operator which can mean addition, if used for numbers.  

But it also means concatenation when applied to a String.  

A String `+` anything else, gives us a String as a result, concatenating anything after the String as text to the initial String.

So if I type:
```java
String myString = "50";
int myInt = 10;
mystring = myString + myInt

System.out.print(myString);
```
We'll get the output : `5010`;  

#### Strings are Immutable
Immutable means that you can't change a String after it's created.

So in the case of the code we've written, the value 10 is technically not appended to the current contents of `myString`.  

Instead, a new String is created automatically by Java. The new String consists of the previous value of myString, plus a textual representation of the integer value 10.  

The net result, is that our variable, myString, has the concatenated value. However, Java created a new String in the process, and the old one will get discarded from memory automatically.

As this process creates a new string every time, its not very efficient and generally not recommended.  


#### String vs StringBuilder

- The String class is immutable, but can be used much like a primitive data type. 

- The StringBuilder class is mutable, but does not share the String's special features, such as being able to assign it a String literal or use the `+` operator on it. 


Both are classes, but the String class is in a special category in the Java language.


> The String is so intrinsic to the Java language, it can be used like a 9th primitive type. But it's not a primitive type at all, it's a class.
{: .prompt-tip }


### Operators, Operands and Expressions

#### What are Operators?

So what are operators?

**<i>Operators in Java are special symbols that perform specific operations on one, two, or three operands, and then return a result.</i>**

In the examples above, which we saw in a previous segment of this document, we used the plus or addition operator, as well as the multiplication operator. 

*Example* : `long longTotal = 50000L + 10L * (byteValue + shortValue + intValue);`

But there are many other operators in Java.

#### What are Operands?

So what is an operand?

An operand is a term used to describe any object that is manipulated by an operator.

So if we consider this:

`int myVar = 15 + 12;`  

The plus here is the operator, and 15 and 12 are the operands. 

Variables used instead of literals can also be operands.  

Another example from a challenge we did previously:  

`long longTotal = 50000L + 10L * (byteValue + shortValue + intValue);`  

In the line above, byteValue, shortValue and intValue are operands, as are the numeric literals.  

#### What are Expressions?

What's an expression?  

An expression is formed by combining variables, literals, method return values, (which we haven't covered yet), and operators.  

They are a way of forming and combining those values to produce a result.  

In the line below, 15 plus 12 is the expression, which returns the value of 27.

`int myVar = 15 + 12;`  

Int the statement below, byteValue + shortValue + intValue is the expression.  

`int sumOfThree = byteValue + shortValue + intValue;`  

### Access Modifier

The `public` Java keyword is what's called an access modifier. 

An access modifier allows us to define which parts of our code, or even someone else's code, can access a particular element.   

```java
public class FirstClass {
    public static void main(String[] args) {
        System.out.print("Hello World");
    }
}
```
### Class Keyword
The **class** keyword is used to define a class. The class name will be the text following the keyword, so **FirstClass** in this case.. 

Notice the **left and right curly braces**, they are used to define the class code block, or class body.

```java
public class FirstClass {
    public static void main(String[] args) {
        System.out.print("Hello World");
    }
}
```
To define a class, requirs an ***optional*** access modifier at the start.

Within a class, we can have data and code.

### Method

```java
public class FirstClass {
    public static void main(String[] args) {
        System.out.print("Hello World");
    }
}
```

You can see, we have this line `public static void main(String[] args)`. Below that we have our `System.out.print("Hello World");` code to print our Hello World message. This is the main method.

**So what is a Methode?**  

A method is a collection of statements, one or more, that perform an operation.

<font color = "#FFCC99"><i>We'll be using a special method called the main method, that Java looks for when running a program.</i></font>

It's the entry point for any Java code, and Java looks for the main method to start and run the program when we use it.

You can also create your own methods.


## In-depth on each topic

### Expressions and Statements

```java
int myVar = 5 + 2;
```
Here there are a total of 2 expressions. `5 + 2` is one of them, and the other is `myVar = 5 + 2`. If we consider `int` and the semi-colon`;` at the end of the line, then `int myVar = 5 + 2;` becomes a vlid Java statement.

Let's look at another example:

```java
int health = 4000;
int score = 650;

if ((health >= 50) && (score >= 100)) {
    score = score + 100;
};
```
Here, there are a total of 7 expressions. They are:
- `health = 4000;`
- `score = 650;`
- `health >= 50`
- `score >= 100`
- `(health >= 50) && (score >= 100)`
- `score + 100`
- `score = score + 100;`

### The Method - in-depth

Java's description of the method is: 

A method declares executable code that can be invoked, passing a fixed number of values as arguments.

#### Benefits of Method

A method is a way of reducing code duplication.  

A method can be executed many times with potentially different results, by passing data to the method in the form of arguments.

#### Structure of the Method

One of the simplest ways to declare a method is shown below.  

This method has a name, but takes no data in, and returns no data from the method (which is what the special word void means in this declaration).

```java
public static void methodName() {
    // Method statements from the method body

}
```

> We have to start our code for a new method outside o another method.
{: .prompt-info }  

> Methods need to be inside a class block. You can't have a method exist on its own, outside of a class' body.
{: .prompt-info }

#### Executing a Method as a Statement

To execute a method, we can write a statement in code, which we say is calling, or invoking, the method.  

```java
boolean gameOver = true;
int score = 800;
int levelCompleted = 5;
int bonus = 100;

int finalScore = score;

if (gameOver) {
    finalScore += (levelCompleted * bonus);
    System.out.println("Your final score was " finalScore);
}
```

For a simple method like `calculateScore`, we just use the name of the method, where we want it to be executed, followed by parentheses, and a semi-colon to complete the statement.  

So for this example, the calling statement would look like the code shown here:

```java
calculateScore();
```

#### Parameters or Arguments

Parameters and arguments are terms that are often used interchangeably by developers.

But technically, a parameter is the definition as shown in the method declaration, and the argument will be the value that's passed to the method when we call it.

```java
public static void calculateScore(int x, int y) {
    // int x, int y are parameters
}


calculateScore(a, b) {
    // a, b are arguments
}
```

#### Executing a Method with parameters

To execute a method that's defined with parameters, you have to pass variables, values, or expressions that match the type, order and number of the parameters declared.

In the calculateScore example, we declared the method with four parameters, the first a `boolean`, and the other three of `int` data types.

So we have to pass first a boolean, and then 3 int values as shown in this statement:

```java
calculateScore(true, 800, 5, 100);
```
*<font color = "#CB3C3C">We can't pass the boolean type in any place, other than as the first argument, without an error.</font>*  


The statement below would cause an error.  

```java
calculateScore(800, 5, 100, true);
```

And you can't pass only a partial set of parameters as shown here. 

This statement, too, would cause an error.

```java
calculateScore(true, 800);
```

#### Method structure with parameters and return type

```java
// Method return type is a declared data type for the data that
// will be returned from the method

public static dataType methodName(p1type p1, p2type p2, {more}) {

    // Method statements
    return value;
}
```
So, similar to declaring a variable with a type, we can declare a method to have a type.  

This declared type is placed just before the method name.  

In addition, a return statement is required in the code block, as shown on the above code block, which returns the result from the method.  

An example of a method declaration with a return type is shown here.  

In this case, the return type is an int.  

```java
public static int calculateMyAge(int dateOfBirth) {
    return (2023 - dateOfBirth)
}
```  
This method will return an integer when it finishes executing successfully.  

#### The Return statement
So, what's a return statement?  

Java states that a return statement returns control to the invoker of a method.  

The most common usage of the return statement, is to return a value back from a method.  

In a method that doesn't return anything, in other words a method declared with void as the return type, a return statement is not required.  

But in methods that do return data, a return statement with a value is required.  

```java
// Here is one way
int highScore = calculateScore(gameOver, score, levelCompleted, bonus);
System.out.println("The highScore is = " + highScore);

// We can also do this
System.out.println("The highScore is = " +
        calculateScore(gameOver, score, levelCompleted, bonus));
```

#### Summary 1:  
- <font color = "FFCC99">We need to use a <b>return statement</b> if we set the method to return a data. Or else, we'll get an error.</font>
- <font color = "FFCC99">We can pass method calls as arguments to other method calls.</font>  
- <font color = "FFCC99">Any method can be executed as an expression.</font>  
- <font color = "FFCC99">A method that returns a value can be used as an expression, or as a part of any expression.</font>  

### More on Methods  

Java's documentation states that:  

A method declares executable code that can be invoked, passing a fixed number of values as arguments.

#### Is the method a statement or an expression?
Like some of the abbreviated operators we learned about, a method can be a statement or an expression in some instances.  

Any method can be executed as a statement.  

A method that returns a value can be used as an expression, or as part of any expression.

#### What are functions and procedures?
Some programming languages will call a method that returns a value, a function, and a method that doesn't return a value, a procedure.  

You'll often hear function and method used interchangeably in Java. 

The term procedure is somewhat less common, when applied to Java methods, but you may still hear a method with a void return type, called procedure.

#### Declaring the Method
So there are quite a few declarations that need to occur as we create a method. 
This consists of:
- Declaring Modifiers. These are keywords in Java with special meanings, we've seen public and static as examples, but there are others.
- Declaring the return type.
    - void is a Java keyword meaning no data is returned from a method.
    - Alternatively, the return type can be any primitive data type or class. 
    - If a return type is defined, the code block must use at least one return statement, returning a value, of the declared type or comparable type.
- Declaring the method name. Lower camel case is recommended for method names.
- Declaring the method parameters in parentheses. A method is not required to have parameters, so a set of empty parentheses would be declared in that case.
- Declaring the method block with opening and closing curly braces. This is also called the method body.


#### Declaring the Parameters
Parameters are declared as a list of comma-separated specifiers, each of which has a parameter type and a parameter name (or identifier).

Parameter order is important when calling the method.

The calling code must pass arguments to the method, with the same or comparable type, and in the same order, as the declaration.

The calling code must pass the same number of arguments, as the number of parameters declared.

#### Declaring the Return Type
When declaring a return type:

`void` is a valid return type, and means no data is returned.
Any other return type requires a return statement, in the method code block.

#### The Return Statement for methods that have a return type
If a method declares a return type, meaning it's not void, then a return type is required at any exit point from the method block.

Consider the method block shown here:  

```java
public static boolean isTooYoung(int age) {
    if (age <  21) {
        return true;
    }
}
```  

So in the case of using a return statement in nested code blocks in a method, all possible code segments must result in a value being returned.

The following code demonstrates one way to do this:  

```java
public static boolean isTooYoung(int age) {
    if (age <  21) {
        return true;
    }
    return false;
}
```  

One common practice is to declare a default return value at the start of a method, and only have a single return statement from a method, returning that variable, as shown in this example method:
  
```java
public static boolean isTooYoung(int age) {
    
    boolean result = false;
    
    if (age <  21) {
        result = true;
    }
    return result;
}
```  

The return statement can return with no value from a method, which is declared with a void return type. 

In this case, the return statement is optional, but it may be used to terminate execution of the method, at some earlier point than the end of the method block, as we show here:

```java
public static void methodDoesSomething(int age) {
    
    if (age <  21) {
        return;
    }
    // Do more stuff here
}
```  

#### The Method Signature
A method is uniquely defined in a class by its name, and the number and type of parameters that are declared for it.

This is called the method signature.

You can have multiple methods with the same method name, as long as the method signature (meaning the parameters declared) are different.

This will become important later in this section, when we cover overloaded methods.


#### Default values for parameters
In many languages, methods can be defined with default values, and you can omit passing values for these when calling the method.

But Java doesn't support default values for parameters.

There are work-arounds for this limitation, and we'll be reviewing those at a later date.

But it's important to state again, in Java, the number of arguments you pass, and their type, must match the parameters in the method declaration exactly.

#### Revisiting the main method
Now, that we're armed with knowledge about methods, we can revisit the main method, and examine it again.

The main method is special in Java, because Java's virtual machine (JVM) looks for the method, with this particular signature, and uses it as the entry point for execution of code.

```java
public static void main(String[] args) {
    // Code in here
}
```  

#### IntelliJ Hint
Finally, in IntelliJ, if you type psvm and hit enter, IntelliJ will insert the main method signature as we show here. 

The only reason to memorize this signature, would be if you were taking a certification exam.

![Alt text](https://i.ibb.co/rwrztbv/Screenshot-2024-01-15-002113.png)


> You can leave a comment & react to my post below using your GitHub account. I added this requirement for GitHub account to avoid spam comments.
{: .prompt-info }  