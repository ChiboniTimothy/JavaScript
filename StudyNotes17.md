# Hoisting in JavaScript

- Hoisting means making some types of varibales accessible/usable in the code before they are actually declared. 
- Hoisting can also be said to be Varibales lifted to the top of their scope

## Behind the scenes 

- Before execution the code is scanned for variables declaration and for each variable found in the code, a new property is created in the variable environment project.

### Different kind of error messages

- ```ReferenceError: can not access 'job' before initialization``` and ```ReferenceError: X is not defined```
- For example:

                Const myName = 'Jonas';

                if(myName === 'Jonas'){
                    console.log(`Jonas is ${job}`)
                    Const job = 'Software Developer';
                    console.log(X);
                }
    
                                                               
function declarations ----  Hoisted - ```Yes```    initial - ```Actual function```      Scope - ```Block```.

Var varibales ---- Hoisted - ```Yes```     initial - ```Undefined```  Scope - ```function```.

let and const varibales ---- Hoisted - ```No```   initial - ```TDZ``` Scope -```Block```.

function expression and arrow ---- ```Depends if using```. 

### Temporal Dead Zone, let and Const

- TDZ makes it easier to avoid and catch errors: accessing variables before declaration is bad and should be avoided.
- TDZ makes ```Const``` variables actually work according to the way there are suppose to be. 

### TDZ in Praactice

                    // this function will be accessible any

-                   function addTwo(a, b){
                        return a + b;
                    }

                    // This function will not be accessible any where else because it's declared by a const

                    Const addTwo = (a, b){
                        return a + b;
                    }

- Variables declared with a ```var``` create a property on a global window object but not with the variable declared with ```const``` or ```let```.
- For example 

                    var X = 1; 
                    console.log(X === window.x)




