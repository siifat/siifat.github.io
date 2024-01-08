---
title: My Java Notes
date: 2024-01-06 13:35:00 +0600
categories: [programing]
tags: [notes]     # TAG names should always be lowercase
---

## <font color="#99FF66">Introduction to Java</font>  

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


## <font color="#99FF66">Requirments to code in Java?</font>
We need a few things to get started.  
- JDK (Java Development Kit)
- An IDE or a Code/Text Editor  

Yep, that's all you need. ✅  

For this guide I'll be using the [Intellij IDEA](https://www.jetbrains.com/idea/download/?section=windows) IDE by JetBrains. But you can use any IDE or Code/Text editor. Some notable ones are [Eclipse](https://www.eclipse.org/downloads/), [NetBeans](https://netbeans.apache.org/front/main/download/index.html) and [Visual Studio Code](https://code.visualstudio.com/).

Now let's write our first code in Java!  

## <font color="#99FF66">Writing our first code</font>
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


## <font color="#99FF66">Terms we need to be clear about</font>  

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
3. ***Optionally***, <font color="purple">add an <b>expression</b> to initialize the variable with a value.</font>

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

## <font color="#99FF66">Before we start</font>  

Before we start our journey of Java, it's crusial to know certain things about it. Below are the things we need to understand to code on Java.  

### <font color="#99FF99">Java Code is case sensitive</font>
Java code is case sensitive.  

**This includes not only keywords and language syntax, but variable names and data types as well.**  

`myFirstNumber` is not the same variable as `MyFirstNumber` with a capital M.  

**int** in lowercase, is not the same as **Int** with the first letter capitalized, or **INT**, all in uppercase, etc.  

**Keywords need to be in lowercase.**  

And **variables will always be exactly as you declare them, including capitalization.**  

<font color="#FFCC66"><i>Remember that, case matters in Java code!</i></font>  


### <font color="#99FF99">How to name a java source file?</font>
- All java source file should end with .java  
    - <font color="#FFCC66"><i>Example : </i></font>`Hello.java`  

- Each .java file can contain only **one public 
class**

- The name of the file should be the name of the public class plus ".java"  
    - <font color="#FFCC66"><i>Example : </i></font>If the public class is `public class HelloWorld` (HelloWorld), then the file name should be `HelloWorld.java`  

> If the class name contains multiple words then capitalize the first letter of each word.  
<i>Example:</i> `HelloWorld.java`
{: .prompt-info }  



> You can leave a comment & react to my post below using your GitHub account. I added this requirement for GitHub account to avoid spam comments.
{: .prompt-info }  