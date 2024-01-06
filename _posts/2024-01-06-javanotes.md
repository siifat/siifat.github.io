---
title: My Java Notes
date: 2024-01-06 13:35:00 +0600
categories: [programing]
tags: [notes]     # TAG names should always be lowercase
---

---

# Introduction to Java

## What is Java?
Java
: Java is a powerful and versatile programming language that has been widely used for over two decades. It's known for its portability, security, and object-oriented approach.

### Key features of Java
- General-Purpose Programming Language
- Easy to learn 
- Write Once, Run Anywhere (WORA)
- Object-Oriented
- Secure
- Platform Independent
- It's Free!


## How to run our first code in Java?
We need a few things to get started.  
- JDK (Java Development Kit)
- An IDE or a Code/Text Editor  

Yep, that's all you need. ✅  


For this guide I'll be using the [Intellij IDEA](https://www.jetbrains.com/idea/download/?section=windows) IDE by JetBrains. But you can use any IDE or Code/Text editor. Some notable ones are [Eclipse](https://www.eclipse.org/downloads/), [NetBeans](https://netbeans.apache.org/front/main/download/index.html) and [Visual Studio Code](https://code.visualstudio.com/).

Now let's write our first code in Java!

## Writing our first code
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
{: .prompt-info }  

**3. `System.out.print("Hello world");`**

- **`System.out.print`:** This part tells Java to print something to the console (the text window where you see the output). It's like using a loudspeaker to speak to the user.
- **`"Hello world"`:** This is the text that you want to print to the console. It's the message you're sending to the user.

**In essence:**

- You're creating a class named `HelloWorld` that acts as a blueprint for your program.
- Inside that class, you have a method named `main` that Java runs when the program starts.
- The `main` method simply prints the message "Hello world" to the console to show that the program ran successfully.

**Congratulations!** 🥳 You've wrote your first Java program!


> You can leave a comment & react to my post below using your GitHub account. I added this requirement for GitHub account to avoid spam comments.
{: .prompt-info }