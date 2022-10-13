### THIS KEYWORD IN JAVASCRIPT

- ```this keyword``` is a special variable that is created for every execution context(every function). 
- It takes the value of (points to) the ```owner``` of the function in which the ```this``` keyword is used.
- The value of this keyword is not static. It depends on how the function is called and it's value is only assigned when the function is actually called.

### 4 Different way in which functions can be called

1. Using a method

- When method is called the ```this keyword``` inside that method will simply point to the object on which the method is called or  point to the  method which is calling the method.

            const jonas = {
                name: 'Jonas',
                year: 2002,
                calAge: function(){
                    return 2037 - this.year;
                    }
                }
            }

            jonas.calAge();

2. Calling the normal function the ```this keyword``` is undefined because has the function has it's own ```this keyword```
3. In the Arrow function the ```this keyword``` is window meaning that inherits the parents and it does not have it's own ```this keyword```.
- Example:

            const jonas = {
                year: 2000,
                calAge: function(birthYear){
                    console.log(2022 - birthYear)
                    console.log(this)
                }
            }

            jonas.calAge(2002);

- When we have the ```this keyword``` inside a method the object is what will be called and rhe name given to the whole objec.
- As illustrated above in the example, the output will be 

                20
                {year: 2000, calAge: [function: calAge]}

- The ```this keyword``` helps in reviewing the object inside a method
- We can also borrow from one method to another 

            const peter = {
                year: 2001
            }

// This allows us to borrow what is in the first method

     peter.calAge = jonas.calAge; 

- This is called method borrowing 