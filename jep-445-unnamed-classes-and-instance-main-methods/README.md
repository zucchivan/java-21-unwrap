# JEP 445: Unnamed Classes and Instance Main Methods (Preview)

## Overview
A feature aimed at simplifying the Java language for students and beginners, or for writing very basic applications. This JEP allows students to write their initial programs without the need to understand complex language features designed for larger programs. By enabling streamlined declarations for single-class programs, JEP 445 offers a smooth transition for students to gradually learn and incorporate more advanced Java features as their skills develop​​.

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

