# Java Quickstart Guide
## Introduction
This guide was built for myself and others as a quick jumpstart into the world of Java programming. This is not an indepth tutorial on how to program in Java, but rather a reference guide for those who may want to try out Java and know other languages.

Feel free to fork and add additional information. 

## Table of Contents
1. [Environment](#Environment)
1. [Starting off your program](#Setting-Up)
1. [Giving your program life](#doing-things)
1. [Java Types](#types)

## Environment
There are many IDEs for Java development. The two most popular IDEs are [Eclipse](http://www.eclipse.org/) and [Netbeans](https://netbeans.org/). **If you are developing for android, please check out [Android Studio](https://developer.android.com/tools/studio/index.html) too.**

## Setting Up
To start a simple project, navigate to your IDE's project creation wizard. For the sake of simplicty, give it the name `helloworld` and name your first project file `helloworld.java`

Once created, your programming environment should either give you the following or a blank space. (If you do get a blank environment, paste the following code down)
```
public class helloworld {
  
}
```

### Deconstructing 
  - `Public`: means that the method is visible and can be called from other objects of other types. Other alternatives are private, protected, package and package-private. See here for more details.
  - `Class`: is essentially an object used in Java. It's used in this case to identify `helloworld` as a `class`.
  - `helloworld`: the name of your class. It should also be the name of your file.

## Doing Things
Let's just make this program say hello world in your console.

```
public class helloworld {
  public static void main(String args[]){
  		System.out.println("hello world");
  }
}
```

### Deconstructing
  - `static`: means that the method is associated with the class, not a specific instance (object) of that class. This means that you can call a static method without creating an object of the class.
  - `void`: means that the method has no return value. This can be interchanged with something like `int` (which returns an integer).
  - `main`: the name of this function. (can be `swaggysunday` if you really wanted it to be)
  - `String Args[]`: See Below
  - `Sytem.out.println`: is a superclass with subclasses that call the class println. Println will push your string into the console.

#### On String Args[]
`String` defines what `args[]` is. `args[]` is a variable (string in this case) that arguments can be used in your function.

For example if the user runs a program called helloworld and types helloworld(hound). This would spit out `hello world hound` if that program was the code below:

```
  public static void main(String dogs){
  		System.out.println("hello world" + dogs);
  }
```

## Types
### Primitives
  When defining a variable, you must add a primative type. (`boolean result = true;`)

  - Integers (with min/man values of each)
    - `byte` (-128 / 127)
    - `short` (-32,768 / 32,768)
    - `int` (-2^31 / (2^31 - 1))
    - `long` (-2^63 / (2^63 -1))
  - Floating Points
    - `float` (32 bit representation)
    - `double` (64 bit representation)
  - Others
    - `boolean`: true or false
    - `char`: a 16 bit unicode character
    - `string`: a string
    
### Arrays
Arrays are essentially lists of things. In real life that could be a list of groceries you need to purchase. 

In java arrays are a bit more constrained than lists, to define an variable as an array, you will need to define a primative with []. An array of of strings would written as `string[] animals = {'dog','cat'}` (defining the variabe animals as an array containing the strings `dog` and `cat`).

To get the `dog` string out of that array we would do this: `animals[0]`.

#### Why start at 0 instead of 1?
In most programming languages counting starts at 0, meaning to get the first object in an array, we need to give [] the input 0.

### Classes
Classes are the containers of Java. They contain the code that allow you perform actions within your Java program. Classes can act as containers for strings, equations, integers, and pretty much anything else in Java. Take the following as an example.

```
public class rectangle {
    public int x = 0;
    public int y = 0;
    //constructor
    public rectangle(int a, int b) {
        x = a;
        y = b;
    }
    
    public int getArea() {
        return x * y;
    }
}
```

This class, `rectangle` contains a few items within it. If we want to access something within a class, such as getArea(), we can type `rectangle.getArea()`
