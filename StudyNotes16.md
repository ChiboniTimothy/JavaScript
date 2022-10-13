# JavaScript High Level

- JavaScript is a high level language which does not have to worry about memory in a computer because it is able to create it's own memory and collect garbage.
- JavaScript is a paradigm language because it contains 3 paradigms namely; ```Procedural programming```, ```object oriented programming```, and ```functional programming```.
- JavaScript is a prototype based object oriented approach language meaning that every element is JavaScript is expected to considered to be an object unless ```numbers```, and ```strings```.
- JavaScript is a language with first class functions and this functions aew treated like variables e.g

            let calcAge = (birthYear){
                let now = 2022 - birthYear;
            };

## JavaScript Engine and Runtime

- JavaScript engine is simply a computer program which executes a JavaScript code. Every browser has it's own JavaScript engine
- For example:

                V8 Engine which powers chrome and nodeJs

- JavaScript engine contains the ```call stack``` and ```Heap```.
- In the call stack, this is where the code is executed while in the heap this is where the objects are stored.

### Compilation vs Interpretation of JavaScript codes

- Compilation is an entire source code which is converted into machine code at once and written to a binary file that can  be executed by a computer.

- Interpretation -- Interpretes runs through the source the source code and executes it line by line.

### Just in Time (JIT) Compilation 

- Is where an entire source code is converted into machine code at once, then executed immediately.

- In this case ```Event Loop``` takes a call back function from the call back queue and put them in a call stack.

### Execution Context

- This is an environment in which a piece of JavaScript code is executed. It stores all the neccessary information for some code to be executed.

- Inside execution context, we have 

1. Variable environment

- ```let```, ```const```, and ```var``` declarations
- ```functions```
- ```arguements object```

2. Scope chain
3. ```this``` keyword

### Scoping and Scope in JavaScript

- ```Scoping``` controls how our program's variables are organized and accessed.

- ```Lexical scoping``` this is scooping which is controlled by placement of functions and blocks in the code.
- ```Scope``` is a space or environment in which a certain variable is declared (Variable environment in case of function).

### Types of scope 

- There are 3 types of scope namely; ```Global scope```, ```function scope``` and ```block scope```.

- ```Global Scope``` is a top level scope. These are variables which are declared out side of any function or block.
- These variables are accessible everywhere 
- For example:

                const me = 'Chiboni';
                Const job = 'Software developer';
                const year = '2022';

- ```Function scope``` These are varivales which are declared inside a function and these are called local scope.
- For example:

                   let calcAge = (birthYear){
                     const age = 2022; 
                     let now = now- birthYear;
                    return now;
                   };

- ```Block scope``` These are varibales which are accessible only inside block (block scope). However, these only applies to ```let``` and ```const``` variables. 

### Scoping in Practice 

- Only inside a scope we are able to access a global varriable and not the other way round.
- Variables inside a function do not have access to those defined as a global scope.