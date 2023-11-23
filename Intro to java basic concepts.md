# Intro to Java

Java is a high-level, general-purpose programming language that is designed to be platform-independent, meaning that Java programs can run on any device that has a Java Virtual Machine (JVM). It was developed by Sun Microsystems (which is now owned by Oracle Corporation) and released in 1995. Java is known for its "write once, run anywhere" philosophy, which means that once you write a Java program, it can run on any device that has a compatible JVM without modification.

Here's a simple example of a basic Java program and an explanation of its typical structure:

```java
// This is a simple Java program

// The class definition
public class HelloWorld {
    // The main method, where the program starts execution
    public static void main(String[] args) {
        // Print a message to the console
        System.out.println("Hello, World!");
    }
}
```

### structure:

1. **Class Declaration:**
   - `public class HelloWorld`: This declares a class named `HelloWorld`. In Java, every application consists of at least one class, and the name of the class must match the name of the file (with the extension `.java`).

2. **Main Method:**
   - `public static void main(String[] args)`: This is the main method. It serves as the entry point for the Java program. When you run a Java program, the JVM looks for this method and starts executing the code inside it. The `args` parameter allows you to pass command-line arguments to your program.

3. **Code Block:**
   - `{}`: The curly braces define a block of code. In this example, the block contains the statements that are executed when the program runs.

4. **Print Statement:**
   - `System.out.println("Hello, World!");`: This statement prints the string "Hello, World!" to the console. The `System.out.println` is a method that outputs text to the console.

To run this program, you would typically follow these steps:

1. Write the code in a text editor and save it with a `.java` extension (e.g., `HelloWorld.java`).
2. Open a command prompt or terminal window.
3. Navigate to the directory where your Java file is located.
4. Compile the Java file using the `javac` command: `javac HelloWorld.java`.
5. Run the compiled program using the `java` command: `java HelloWorld`.

After running these commands, you should see the output "Hello, World!" printed to the console.


### Variable:
A variable in programming is a storage location identified by a memory address and an associated symbolic name (an identifier), which contains some known or unknown quantity of information referred to as a value. In simpler terms, a variable is a way to store and manipulate data in a program. Variables have a data type (e.g., integer, floating-point, string) that determines the kind of data they can hold.

### Data Types in Java:
Java is a strongly-typed programming language, which means that variables must be declared with a specific data type before they can be used. Here are some common data types in Java:

1. **Primitive Data Types:**
   - `int`: Integer (whole numbers)
   - `double`: Double-precision floating-point (decimal numbers)
   - `float`: Single-precision floating-point
   - `char`: Character (single Unicode characters)
   - `boolean`: Boolean (true or false)

2. **Reference Data Types:**
   - `String`: Represents sequences of characters (text)
   - `Object`: The root class for all Java classes
   - Arrays: Collections of elements of the same type

### Operators in Java:
Operators in Java are symbols that perform operations on variables and values. They are used to manipulate data and perform calculations. Here are some common types of operators:

1. **Arithmetic Operators:**
   - `+` (addition)
   - `-` (subtraction)
   - `*` (multiplication)
   - `/` (division)
   - `%` (modulo - remainder after division)

2. **Comparison Operators:**
   - `==` (equal to)
   - `!=` (not equal to)
   - `<` (less than)
   - `>` (greater than)
   - `<=` (less than or equal to)
   - `>=` (greater than or equal to)

3. **Logical Operators:**
   - `&&` (logical AND)
   - `||` (logical OR)
   - `!` (logical NOT)

4. **Assignment Operators:**
   - `=` (assignment)
   - `+=`, `-=`, `*=`, `/=` (compound assignment)

### Java Classes and Objects:
In Java, a class is a blueprint for creating objects. Objects are instances of classes and represent real-world entities. A class defines the properties (fields) and behaviors (methods) that its objects will have. Here's a basic example:

```java
// Define a simple class
public class Car {
    // Fields (properties)
    String brand;
    int year;
    
    // Methods (behaviors)
    void start() {
        System.out.println("The car is starting.");
    }
    
    void drive() {
        System.out.println("The car is in motion.");
    }
}

// Create an object of the class
Car myCar = new Car();

// Access fields and methods of the object
myCar.brand = "Toyota";
myCar.year = 2023;
myCar.start();
myCar.drive();
```

In this example, `Car` is a class with fields (`brand` and `year`) and methods (`start` and `drive`). `myCar` is an object of the `Car` class, and you can access its properties and methods using dot notation.

**Object-Oriented Programming (OOP):**

Object-Oriented Programming (OOP) is a programming paradigm that revolves around the concept of "objects." An object is a self-contained unit that consists of both data (attributes or properties) and procedures (methods or functions) that operate on the data. OOP is based on a few fundamental principles that help in designing and organizing code in a modular and reusable way.

### Core Features of OOP:

1. **Encapsulation:**
   - Encapsulation refers to the bundling of data (attributes) and the methods (functions) that operate on the data into a single unit or class. It helps in hiding the internal details of an object and exposing only what is necessary.

2. **Inheritance:**
   - Inheritance is a mechanism that allows a new class (subclass or derived class) to inherit properties and behaviors from an existing class (superclass or base class). This promotes code reuse and establishes a relationship between classes.

3. **Polymorphism:**
   - Polymorphism allows objects of different classes to be treated as objects of a common superclass. It enables a single interface to represent entities of different types and provides a way for objects to take on multiple forms.

4. **Abstraction:**
   - Abstraction involves simplifying complex systems by modeling classes based on their essential characteristics. It allows the programmer to focus on the relevant details of an object while ignoring unnecessary complexities.

### Other Features of OOP:

1. **Modularity:**
   - OOP promotes modularity by breaking down a complex system into smaller, more manageable parts (objects). Each object can be developed, tested, and maintained independently, making the codebase easier to understand and maintain.

2. **Message Passing:**
   - Objects communicate with each other by sending messages. A message typically involves invoking a method on an object, and this method call triggers the execution of the corresponding code within the object.

3. **Association:**
   - Association represents the relationships between classes. It describes how objects interact with each other. Associations can be one-to-one, one-to-many, or many-to-many, reflecting the connections between different objects.

4. **Composition:**
   - Composition is a form of association where one class contains an object of another class. It allows for creating complex objects by combining simpler objects, promoting code reuse and flexibility.

5. **Overloading and Overriding:**
   - Overloading involves defining multiple methods in the same class with the same name but different parameter lists. Overriding occurs when a subclass provides a specific implementation for a method that is already defined in its superclass.

These features collectively contribute to the principles of OOP and help in creating software that is modular, flexible, and easy to maintain. OOP is widely used in modern programming languages such as Java, C++, and Python.

**Introduction to Decision Control:**

Decision control structures in programming allow the execution of different code segments based on certain conditions. These conditions are evaluated to either true or false, and the program takes different paths accordingly. Decision control is essential for building flexible and responsive programs.

### If Statement:

The `if` statement is a fundamental decision-making statement. It allows a program to execute a certain block of code if a specified condition is true. The syntax in many programming languages is as follows:

```java
if (condition) {
    // Code to be executed if the condition is true
}
```

### If-Else Statement:

The `if-else` statement extends the `if` statement by providing an alternative block of code to be executed when the condition is false. The syntax is:

```java
if (condition) {
    // Code to be executed if the condition is true
} else {
    // Code to be executed if the condition is false
}
```

### Nested If Statement:

Nested `if` statements involve placing one `if` statement inside another

```java
import java.util.Scanner;

public class NestedIfExample {
    public static void main(String[] args) {
        // Create a Scanner object to read input
        Scanner scanner = new Scanner(System.in);

        // Prompt the user to enter age
        System.out.print("Enter your age: ");
        int age = scanner.nextInt();

        // Check if the person is of voting age
        if (age >= 18) {
            System.out.println("You are eligible to vote.");

            // Ask the user about citizenship
            System.out.print("Are you a citizen? (yes/no): ");
            String citizenship = scanner.next().toLowerCase();

            // Nested if to check citizenship
            if (citizenship.equals("yes")) {
                System.out.println("You are eligible to vote in the elections.");
            } else if (citizenship.equals("no")) {
                System.out.println("Sorry, you must be a citizen to vote.");
            } else {
                System.out.println("Invalid input for citizenship. Please enter 'yes' or 'no'.");
            }
        } else {
            System.out.println("Sorry, you are not eligible to vote as you are under 18 years old.");
        }

        // Close the scanner
        scanner.close();
    }
}
```

In this example:

1. The program asks the user to enter their age.
2. If the age is 18 or older, it proceeds to ask about citizenship.
3. Depending on the citizenship status, it prints a message about whether the person is eligible to vote or not.
4. If the age is less than 18, it informs the user that they are not eligible to vote.

This is a simple example of nested `if` statements where the decision-making process involves multiple conditions.