# C# Basic

## .NET
* CLR (Common Language Runtime)
* Class Library

### CLR
An application that translate IL (intermediate language, similar to Java's bytecode) in to machine language (just-in-time compilation).

This is what makes C# a cross-platform language. 

### Architecture
From the bottom of the hierarchy and up.

Classes -> Namespaces -> Assembly -> Application.
```
namespace HelloWorld {
    class Program {
        static void Main(string[] args){
            code...
        }
    }
}
```

To use a class from a different namespace -> import it with 'using' statement.

