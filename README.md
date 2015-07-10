# Java Quickstart Guide
## Introduction
This guide was built for myself and others as a quick jumpstart into the world of Java programming. This is not an indepth tutorial on how to program in Java, but rather a reference guide for those who may want to try out Java and know other languages.

Feel free to fork and add additional information. 

## Table of Contents
1. [Environment](#Environment)
1. [Setting Up](#Setting-Up)
1. [Doing Things](#doing-things)

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
  - `Public` - means that the method is visible and can be called from other objects of other types. Other alternatives are private, protected, package and package-private. See here for more details.
  - `Class` - is essentially an object used in Java. It's used in this case to identify `helloworld` as a `class`.
  - `helloworld` - the name of your class. It should also be the name of your file.

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
  - `static` - means that the method is associated with the class, not a specific instance (object) of that class. This means that you can call a static method without creating an object of the class.
  - `void` - means that the method has no return value. This can be interchanged with something like `int` (which returns an integer).
  - `main` - the name of this function. (can be `swaggysunday` if you really wanted it to be)
  - `String Args[]` - See Below

#### On String Args[]
`String` defines what `args[]` is. `args[]` is a variable (string in this case) that arguments can be used in your function.

For example if the user runs a program called helloworld and types helloworld(hound). This would spit out `hello world hound` if that program was the code below:

```

  public static void main(String dogs){
  		System.out.println("hello world" + dogs);
  }
```
