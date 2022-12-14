# yoLang
A very simple idea of "Programming language" written using Javascript on Web

CAUTION: THIS IS NOT A REAL PROGRAMMING LANGUAGE!

## Try It

https://madcoderme.github.io/yoLang/

Hi fellow **engineers**! 👋

A lot of programmers have the dream to create their own Programming Language. To be honest, this is not an easy deal, especially if you are just starting to learn this thing called "Coding".

**Yo** (Don't mess up with YODev) is a project built to have fun. It is not a serious language. I even struggle to call it a language because
- It translates code to Javascript
- It runs on a HTML file
- Yes, The compiler lives in a HTML file

Anyway, please consider this as a project to think in a new way, to get new experience and to spend time in another fun project.

## How does it work?
There are three parts -

- **Input TextArea:** This takes the code as input (No code formatting sadly)
- **Output Area:** This is where the output is displayed along with compiling information. You can think this as a Terminal.
- **Interpreter:** Every language needs a compiler or interpreter to translate your code to something that computer can understand. This part of the project translates the Yo code to Javascript. Yo compiler goes line by line and converts the code to executable programme.

## Syntax
I love the syntax of C++, C#, Java and Javascript. I also like the simplicity of Python.
So, I decided to make the syntax a combination of those.

### Data Types
Yo has support for all those Data types you can see in the languages mentioned above.

```
10                            // This is a number
'Hello world'                 // This is a String. Strings must be inside single quotation. 
true                          // This is a boolean value
[1, 2, 3]                     // This is an Array
{ name: 'Yo', age: '1 Day' }  // This is an Object

```

### Mathematical Operations
You can expect the most basic stuffs here only. So, Yo offers you all those basic operations -

```
1 + 1
2 - 1
5 * 6
8 / 2
2 ** 3
```
Here is the reason of giving this simple thing a different section. Sometimes, if you want to perform a mathematical addition, you may end up with unexpected result like this - 

```
print 1 + 1 
// Output: 11
```
This is mainly because of the compiling process. To avoid this, you should do all mathematical operations inside Parenthesis. 

```
print (1 + 1) 
// Output: 2
```

### Variable Declaration
To declare a variable, you need to use the keyword `#` - 

```
#a = 10
#b = 20
```

Remember, Yo is very sensitive about spaces at this moment. So you must put those two spaces, before and after the equal(=) sign.

You can also declare constants. To do this, you need to use the keyword `c#`

```
c#SuperImportantVal = 'A constant value'
```

To update the value of a variable, you can simply write this - 

```
#a = 'Hello'
a = 'Hello world'
```

### Functions
To write a function, you need to use the keyword `f#`

```
f# sayHello[] (
  return 'hello'
)
```
Then, you can call the function simply - 
```
sayHello()
```

Parameters can be passed between the square brackets.

```
f# addTwoNumbers [num1, num2] (
  return num1 + num2
)

addTwoNumbers(5, 7) //This should return 12
```

### Classes
To write a class, use the keyword `class#`. To declare methods, use the keyword `m#`

```
class# Box (
   m# constructor [color] (
      this.color = color
   )
   
   m# getColor [] (
      return this.color
   )
)
```

You can use this Class as you do in JS.

```
#b = new Box('red')
print b.getColor()
```

### Conditional Statements (If else)
You almost can't think of a programming language without if else these days. The way to write if statement in Yo is -

```
#a = 10
#b = 15

if a > b (
  print 'a is bigger'
) else (
  print 'a is smaller'
)
```
Note that we are using Paranthesis instead of Curly Brackets. Also, the condition is not wrapped inside brackets. 

At this moment, only the following conditions are supported - 

```
a == b
a != b
a > b
a < b
```
So, No AND OR statements :)

**Make sure you put those spaces as shown above. Yo is Space sensitive!**

### Loops
At this moment, only a `for loop` is supported. But the way to write this is different. 

```
loop i, 0, 10, 1 (
  print i
)
```

This should print numbers from `0` to `9`. Basically, the syntax is - 

```
loop [variable name], [starting num], [ending num], [increment value] (

)
```

## Writing a Hello World Programme

You can expect to be fairly easy my boy:

```
print 'Hello World!'
```

### Dive deeper

Using the built in `print` function, you can display Strings in the Output terminal. If you pass a Number or any other data type, those will be automatically converted to string. Only in case of an Object, this will return `[object Object]` For example - 

```
#testNum = 10
#testStr = 'is Ten'

print testNum + ' ' + testStr // It will print "10 is Ten"
```

