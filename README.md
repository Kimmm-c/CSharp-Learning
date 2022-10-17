# C# Basic

## .NET
* CLR (Common Language Runtime)
* Class Library

### CLR
An application that translate IL (intermediate language, similar to Java's bytecode) in to machine language (just-in-time compilation).

This is what makes C# a cross-platform language. 

### Architecture
From the bottom of the hierarchy and up: Classes -> Namespaces -> Assembly -> Application.
```
using System;

namespace HelloWorld {
    class Program {
        static void Main(string[] args){
            code...
        }
    }
}
```

To use a class from a different namespace -> import it with 'using' statement.

## Overflowing
```
byte number = 255;
number = number + 1;    //0
```
The boundary of a byte is [0, 255]. Trying to increase number by 1 will result in overflowing and unexpectable output.

Use `checked` to check for the boundary. The exception will be thrown and the program will crash.
```
checked {
    byte number = 255;
    number = number + 1;    //0
}
```

## From from statically type to dynamically type
Use keyword `var` in replacement for data type keyword and let the compiler detect the data type of a variable automatically. 

Note that number will be interpreted as int. 
```
var number = 2; //this will be an int
var letter = 'a';
```

