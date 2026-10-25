# Chapter 2 — Intermediate

Now that you know the basics, let's level up.

## Loops

### while
```cajyu
var i = 0;
while i < 5 {
  print(i);
  i = i + 1;
}
```

### for
```cajyu
for i in range(5) {
  print(i);
}
```

## Libraries

Install a library:
```bash
cajyu inst serial
```

Then use it:
```cajyu
import print from CajyuLibs.serial;
print("Hello from a library!");
```

## try / catch

```cajyu
const result = try 10 / 0;

catch result {
  print("Something went wrong");
}
```

## String Manipulation

```cajyu
import str from CajyuLibs.string;

print(str.upper("hello"));
print(str.split("a,b,c", ","));
```

## JSON

```cajyu
import json from CajyuLibs.json;

var text = '{"name":"Cajyu"}';
var obj = json.parse(text);
print(obj.name);
```

## Files (fs)

```cajyu
import fs from CajyuLibs.fs;

fs.writeFile("hello.txt", "Hello!");
var content = fs.readFile("hello.txt");
print(content);
```

## ReadLine — Ask for a name

```cajyu
import input from CajyuLibs.ReadLine;
import print from CajyuLibs.serial;

var name = wait input("What is your name? ");
print("Hello, " + name + "!");
```

## Debugging with serial

```cajyu
import print from CajyuLibs.serial;

print("Debug: value is " + someValue);
```

Next: [Chapter 3 — Advanced Libraries](../Chapter-3/)
