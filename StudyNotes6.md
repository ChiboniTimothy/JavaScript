### CONTINUATION OF FUCNTIONS

- A function can be called inside another function by asssigning in storing it in a variable. 
- For example:

                const fruitCuttingBusiness = fruits => {
                    return fruits * 3;
                            };

                const juiceProduction = (apples, mangos) => {
                const choppedApples = fruitCuttingBusiness(apples);
                const choppedMangos = fruitCuttingBusiness(mangos);
                const juice = `I want ${choppedApples} pieces of apples juice and ${choppedMangos}      pieces of mangos juice.`; 
                    return juice;
                }

                console.log(juiceProduction(4, 5));

### TYPES OF FUNCTIONS

- There are 3 types of functions namely, Function Declaration, Function Expression and Arrow Function.
- Function declaration is a function which can be used before it is  declared.
- Example:

            function calAge(year){
                return 2022 - year;
            };

- Function expression these are functions which are stored in a variable 
- Example:

            const calAge = fucntion(year){
                return 2022 - year;
            };

- Arrow function these are functions which are great for a quick one-line function and they do not have a this keyword.
- Example:

            const calAGE = year => 2022 - year;

- Function can be written different ways  but they all work in a similar way like receiving data input, transforming data as well as outputting data.
- Parameters are placeholders which receive input values.
- parameters are like local variables of a function.
- return is a statement to output a value from the function and it terminates the execution of the function.

### ARRAYS

- Arrays help in storing data in a variable that can be used later on.
- Arrays can be written in two different ways 
- For example:

                const friends = ["Martin", "John", "Grace"];

                or
                  // This is actually called array function

                const years = new Array(2022, 2021, 2020);

- Elements can be extracted from an array
- For example:

                const friends = ["Peter", "Holding", "Goldon"];
                console.log(friends[0])

- With arrays you are able to know the number of elements in an array
- For example:

                
                const friends = ["Peter", "Holding", "Goldon"];
                console.log(friends.length)

- You can acquire the last element in an array
- For example:


                const friends = ["Peter", "Holding", "Goldon"];
                console.log(friends[friends - 1]);

- You can replace elements  in array
- For example:

                const friends = ["Peter", "Holding", "Goldon"];
                friends[2] = "Stephen";
                console.log(friends);

- Arrays are able to hold different types of data and they allow you to have an array inside an array
- For example:

                const Car = ["Jonas", "Simponson", 2022 - 1990, "Terry", friends];
                console.log(Car);

### ARRAY OPERATIONS

- There are few array operations such as ```Push method```, ```Unshift method```, ```Pop method```, ```Shift method```, ```indexOf```, ```includes```.

- Push method add an element to the end of an array
- For example:

                 const friends = ["Peter", "Holding", "Goldon"];
                 friends.push('Jay');
                 console.log(friends);

                // Result will be ["Peter", "Holding", "Goldon", "Jay"];

- Unshift method adds an element at the beginning of an array;
- For example:

                 const friends = ["Peter", "Holding", "Goldon"];
                 friends.unshift('Jay');
                 console.log(friends);

                 // Result will be ["Jay", "Peter", "Holding", "Goldon",]   

- Pop method removes the last element of an array
- For example:

                  const friends = ["Peter", "Holding", "Goldon", "Jay"];
                 friends.pop('Jay');
                 console.log(friends);

                 // Result will be ["Peter", "Holding", "Goldon",]

- Shift method removes the first element  of an array
- For example:

                 const friends = ["Peter", "Holding", "Goldon"];
                 friends.shift('Jay');
                 console.log(friends);

                 // Result will be ["Holding", "Goldon", "Jay"];

- IndexOf ('element name') method returns the position of an element in an array.
- For example:
                 
                 const friends = ["Peter", "Holding", "Goldon"];
                 console.log(friends.indexOf("Peter"));

                 // Result will be 0

- Include is new method produced in the ```ES6``` which tells a boolean of the element passed.
- For example:


                 const friends = ["Peter", "Holding", "Goldon"];
                 console.log(friends.includes("Peter"));

                 // Result will be true

