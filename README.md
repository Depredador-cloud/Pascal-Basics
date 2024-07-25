# Pascal-Basics

# Pascal Programming Guide

## Table of Contents
1. [Introduction](#introduction)
2. [History of Pascal](#history-of-pascal)
3. [Getting Started with Pascal](#getting-started-with-pascal)
4. [Basic Syntax and Structure](#basic-syntax-and-structure)
5. [Data Types](#data-types)
6. [Operators](#operators)
7. [Control Structures](#control-structures)
8. [Procedures and Functions](#procedures-and-functions)
9. [Advanced Topics](#advanced-topics)
10. [Sample Programs](#sample-programs)
11. [Resources](#resources)

## Introduction
Pascal is a high-level programming language developed by Niklaus Wirth in the late 1960s. It was named after the French mathematician Blaise Pascal and was designed to encourage good programming practices using structured programming and data structuring.

## History of Pascal
Pascal was designed to teach programming as a systematic discipline and to develop reliable and efficient programs. It became popular in the 1970s and 1980s for teaching programming in schools and universities.

## Getting Started with Pascal
To start programming in Pascal, you need a Pascal compiler. Free Pascal (FPC) and Turbo Pascal are two commonly used compilers.

### Installing Free Pascal
1. Download Free Pascal from [Free Pascal website](https://www.freepascal.org/).
2. Follow the installation instructions for your operating system.

## Basic Syntax and Structure
A Pascal program consists of a heading, a declaration part, and a statement part.

```pascal
program Example;
var
  a, b, c: integer;
begin
  a := 10;
  b := 20;
  c := a + b;
  writeln('Sum of a and b: ', c);
end.
```

## Data Types
Pascal has several standard data types:

- **Integer**: Whole numbers
- **Real**: Floating point numbers
- **Char**: Single characters
- **String**: Sequences of characters
- **Boolean**: True or false values

### Example
```pascal
var
  i: integer;
  r: real;
  c: char;
  s: string;
  b: boolean;
```

## Operators
Pascal supports various operators for arithmetic, relational, logical, and bitwise operations.

### Arithmetic Operators
- `+` : Addition
- `-` : Subtraction
- `*` : Multiplication
- `/` : Division
- `div` : Integer division
- `mod` : Modulus

### Example
```pascal
var
  a, b, result: integer;
begin
  a := 10;
  b := 3;
  result := a div b;  // result is 3
end.
```

## Control Structures
Pascal includes standard control structures such as conditional statements, loops, and case statements.

### Conditional Statements
```pascal
if condition then
  statement
else
  statement;
```

### Loops
#### For Loop
```pascal
for i := 1 to 10 do
  writeln(i);
```

#### While Loop
```pascal
while condition do
  statement;
```

#### Repeat Loop
```pascal
repeat
  statement;
until condition;
```

### Case Statement
```pascal
case selector of
  1: statement;
  2: statement;
  else statement;
end;
```

## Procedures and Functions
Pascal allows the use of procedures and functions for code modularity.

### Procedures
```pascal
procedure DisplayMessage;
begin
  writeln('Hello, World!');
end;

begin
  DisplayMessage;
end.
```

### Functions
```pascal
function Add(a, b: integer): integer;
begin
  Add := a + b;
end;

begin
  writeln(Add(5, 3)); // Output: 8
end.
```

## Advanced Topics
### Arrays
```pascal
var
  arr: array[1..5] of integer;
begin
  arr[1] := 10;
  arr[2] := 20;
  // and so on...
end.
```

### Records
```pascal
type
  Person = record
    name: string;
    age: integer;
  end;

var
  p: Person;
begin
  p.name := 'John';
  p.age := 30;
end.
```

### Pointers
```pascal
var
  ptr: ^integer;
  num: integer;
begin
  num := 10;
  ptr := @num;
  writeln(ptr^); // Output: 10
end.
```

### File Handling
```pascal
var
  f: Text;
begin
  Assign(f, 'example.txt');
  Rewrite(f);
  writeln(f, 'Hello, File!');
  Close(f);
end.
```

## Sample Programs
### Hello World
```pascal
program HelloWorld;
begin
  writeln('Hello, World!');
end.
```

### Factorial Calculation
```pascal
program Factorial;
var
  num, i, factorial: integer;
begin
  num := 5;
  factorial := 1;
  for i := 1 to num do
    factorial := factorial * i;
  writeln('Factorial of ', num, ' is ', factorial);
end.
```

## Resources
- [Free Pascal](https://www.freepascal.org/)
- [Turbo Pascal](https://www.embarcadero.com/products/turbo-pascal)
- Books:
  - "Computer Mathematics using Pascal" by Stephen J. Sugden and John Simmond
  - "Software Tools in Pascal" by Brian W. Kernighan and P.J. Plauger
  - "Object Pascal Handbook" by Marco Cantù

---

Feel free to edit and expand this guide based on your specific needs and preferences.
