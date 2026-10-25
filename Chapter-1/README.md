# Chapter 1 — Basics

Welcome to Cajyu! In this chapter you will learn the fundamentals.

## Hello World

```cajyu
import print from CajyuLibs.serial;

print("Hello, world!");
```

## Variables

```cajyu
var name = "Cajyu";
var age = 1;
var active = true;
```

Use `const` when the value should not be reassigned:

```cajyu
const PI = 3.14159;
```

## Arithmetic

```cajyu
var sum = 10 + 5;
var product = 4 * 3;
var result = (10 + 2) / 2;
```

## if / elif / else

```cajyu
var x = 7;

if x > 10 {
  print("big");
} elif x > 5 {
  print("medium");
} else {
  print("small");
}
```

## Functions

```cajyu
fn add a, b {
  return a + b;
}

print(add(2, 3));
```

## Value Types

You can optionally add types:

```cajyu
var name:String = "Cajyu";
var age:Number = 17;
var items:Array = [1, 2, 3];
```

## Classes

```cajyu
class Person {
  Main name, age {
    Self.name = name;
    Self.age = age;
  }
  greet {
    return "Hello, " + Self.name;
  }
}

var p = new Person("Alex", 20);
print(p.greet());
```

## Built-ins — A Helping Hand

Cajyu gives you some useful functions out of the box:

```cajyu
print(len("hello"));      // 5
print(range(5));           // [0, 1, 2, 3, 4]
```

Next: [Chapter 2 — Intermediate](../Chapter-2/)
