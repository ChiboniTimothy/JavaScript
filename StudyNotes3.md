# OBJECTS IN JAVASCRIPT

- Objects in JavaScript are the biggest building block and almost everything in JavaScript is an object.

- Objects are used for collections of data or collections of functionality.

- An object can be created using two curly brackets and a semi colon. 

- Curly brackets and a semi colon is the most common way to make an object, but there are other ways that we will go over.

- const person = {};
- Inside of the person object, you have what are called properties and values. Add the following to types.js 
- For example: 

                        const person = {
                        first: "wes",
                        last: "bos",
                        age: 100,
                        };


- In the console, if you type person it will return the value, which is the object. 
- If you check the type of the person variable, it will return the object type.

### TYPES - NULL AND UNDEFINED

- Undefined

   - If you create a variable and don't set anything to it, it will be alled undefined. 
- For example:

                 let dog;
                     console.log(dog);

- Not assigning a variable to anything results in being an undefined variable

- Undefined is something that has been created (a variable), but has not yet been defined (given a value).

- The same thing goes for properties on an object. If you type in the console person.dog it will return undefined.

- Null

- Null is a value of nothing, whereas undefined is a variable that has not yet had a value set to it.

- For example: 

                let somethingUndefined;
                      const somethingNull = null;

- NOTE: you cannot use a const variable without setting a value.

- somethingUndefined is undefined because it does not have a value set, whereas somethingNull has the value of null, which is nothing. 
- They are both nothing, but in different ways.
- For example:

                 Luko and Chiko (both of who are real people), who we will represent in objects like; 

                        const Luko = {
                           first: "Luko",
                            };

                          const Chiko = {
                                          first: "Raymond",
                                          last: "Chiko",
                                        };

                                           Chiko.first = "Chiko";
                                           Chiko.last = null;

- In this example, Luko never had a last name, so she does not have the last property in her object.

- Luko on the other hand, got rid of his last name, so we are explicitly setting it to null.

- In the console, if you type Chiko.last you will see the value of undefined returned. When you try Luko.last, the value of null wil be returned.


### TYPES - BOOLEANS AND EQUALITY

- Boolean

    - A boolean is either true or false.
    - Booleans are used for logic such as if statements in our JavaScript code.
    - Booleans can be manually set or calculated.
    - For example: 
                    let isDrawing = false;
                    
    - In the above example, let's say we want to know if the user is moving their mouse and if they are currently clicking down or up.
    - To do that, we can use a flag variable, which is a variable that is either set to true or false.
    - When the user clicks down, we set it to true and when they click up, we set it to false. That is what a boolean is -- something that is either true or false.
    - Booleans can be calculated as 
    - For example, if we have an age variable that is set to 18, and another variable called ofAge that has the value of age > 19, if you console log ofAge, it will return false.

                    const age = 18;
                    const ofAge = age > 19;
                    console.log(ofAge);

    - Comparing age as 18 greater than ofAge as 19 results in false
    - Sometimes values are calculated, like for ofAge.

- Equality

  - Equality (equal sign, double equal sign, triple equal sign)

  - One equal sign = is used to assign a value to a variable.

  - For example:

              const age = 100;

  - For double equals == and triple equals ===, know that you should almost always be using triple equals.

  - There are some edge cases where you can use double equals, but almost all the time it's better to use triple equals.

  - If you take the age variable in the console and do the following

  - The use of triple equal operator to compare age with 100

  - age === 100 will return true
  - age === 10 will return false

  - You have 1 value, which can be a straight up value 100 === 10 or it can be a value that is stored in a variable age === 100 or it can be two variables.

# FUNCTIONS

- Functions allow us to group together sets of statements.
- Functions perform some work (a statement), and sometimes they also return a value.
- For example: 

               Math.max(10, 12)
               return will be 12;

- Math.max(10, 12) is a JavaScript statement. The values 10 and 12 that we are passing into the function are called arguments.
- If you are passing multiple values to a function, you need to separate each value with a comma and it's best practice to include a space between each.
- Sometimes, functions will return to you some data that is generally the answer or the computed output based on what you passed in.
- For example:

                 Math.floor(2.4444) will return 2.
- Here we are passing one argument of 2.4444 and it returns to us the floor of that value which is 2.
- parseFloat() which takes in a string and returns a number, it switches the type. 
- For example:

                parseFloat("20.34543543");

- parseInt() takes in a string and returns a number without a decimal 20. 
- For example:

                 parseInt("20.3243423");
- If you type Date.now() in the console it will return something like the following 
- For example: 

                Date.now()
                return 1560268110755

- Date.now() is a function that does not take in any arguments. 
- What it returns to us is the number of milliseconds since January 1, 1970.