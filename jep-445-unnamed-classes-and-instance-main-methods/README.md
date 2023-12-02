# JEP 445: Unnamed Classes and Instance Main Methods (Preview)

## Overview
A feature aimed at simplifying the Java language for students and beginners, or for writing very basic applications. This JEP allows students to write their initial programs without the need to understand complex language features designed for larger programs. By enabling streamlined declarations for single-class programs, JEP 445 offers a smooth transition for students to gradually learn and incorporate more advanced Java features as their skills develop​​.

When launching a class, the launch protocol chooses the first of the following methods to invoke:

1. A `static void main(String[] args)` method of non-private access (i.e., `public`, `protected` or package) declared in the launched class,
2. A `static void main()` method of non-private access declared in the launched class,
3. A `void main(String[] args)` instance method of non-private access declared in the launched class or inherited from a superclass, or, finally,
4. A `void main()` instance method of non-private access declared in the launched class or inherited from a superclass.

## HelloWorld.java
`HelloWorld.java` contains a sample of a very simple main method making use of the features introduced by JEP 445. 

## Compiling
JEP 445 is a preview feature in Java 21, requiring the `--enable-preview` flag during both compilation and execution.

To compile `HelloWorld.java`:

```sh
javac --release 21 --enable-preview HelloWorld.java
```

## Running
After compilation, run the program with:


```sh
java --enable-preview HelloWorld
```

