## CONTINUATION OF FUCNTIONS

- Functions can do anything and functions actually give real power to javascript when you define your own function.
- Functions are created or defined, and they are later called.
- When a function is made and you later want to run the function, this procedure is called calling or running of a function.
- First you type function and then the name of the function. Function naming follows the exact same rules as variable naming which we went over in a previous video.
- For example:

                Let's name this function headDOM 

                     function headDOM() {
                                           // this is a function body
                                            };

- In the above example, I have defined a function named headDom with parenthesis, and open and close fucntion block 
- Note: Anything that goes inside the function block is called the function body, and is part of the function.
- Now in the function body, i will add:

                                        console.log("Running head Dom!!!");

- Open index.html and in the browser and open the console. 
- Try typing headDom in the console and hitting enter.
- To run the function we need to enter into the console headDom(), which will log Running head Dom!!!! in the console.
- A function works just like a variable in that you can call them by the name of it. 
- However, when you put just the name of the function, you see the entire code, as shown above.
- we can run this other function;
- For example:


                    // function definition

                        function Counter() {

                    // this is the function body

                            console.log("Running Hello World!!");
                            }
 

- Let's try to take in the following arguments, and the function should return to us the total value:
  - how much the dinner was
  - the tax rate
  - how much you want to tip

- How this will work is that, we will assume the meal is 100 dollars, and we will multiply it by 1.13 because in Lusaka the tax rate is 13%.
- Example: 

                // function definition

                       let  total = 100 * 1.13;

                    function HeadDom() {

                // this is the function body
                   
                    return result;

                    }
                // Answer when you type result in console will be 113

### FUNCTION INVOCATION

- The code inside the function will execute when "something" invokes (calls) the function
- When an event occurs (when a user clicks a button)
- When it is invoked (called) from JavaScript code
- Automatically (self invoked)

### FUNCTION RETURN

- When JavaScript reaches a return statement, the function will stop executing.

- If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

- Functions often compute a return value. 
- The return value is "returned" back to the "caller":

- Example:

          // Function is called, return value will end up in x

        let x = headDom(4, 3); 

            function headDom(a, b) {

                 // Function returns the product of a and b
                    }
                return a * b;   

                // The result in x will be: 12

