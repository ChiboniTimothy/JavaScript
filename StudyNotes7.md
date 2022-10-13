### USING FUNCTIONS AND ARRAY

- In Javascript it possible to pass an array as a parameter in a function
- To pass an array as a parameter in a function, you first need to create a function  then pass a parameter and return it.
- After creating a function you then need to create an array outside the function
- After creating an array, you then need to create a variable which will store a function with an array  passed as a parameter.
- Example:

                const calAge = birthYear => 2022 - birthYear;
                const years = [2000, 2001, 2002, 2003, 2004];
                const age1 = calAge(years[0]);
                console.log(age1);

                // Answer will be 2022 - 2000 = 22;

### INTRODUCTION TO OBJECTS 

- JavaScript object is defined and created with an object literal
- Objects are used for creating unstructured data while array are used for structured data.
- Example of an object:

                            const profileDetails = {
                                firstName: 'Peter',
                                lastName: 'Banda',
                                age: 2022 - 2002,
                                friends: ['John', 'Kelvin', 'Chanda', 'Kabwe']
                            };

                            console.log(profileDetails);

- You can modify the data in a JavaScript object
- Example:

                    const profileDetails = {
                    firstName: 'Peter',
                    lastName: 'Banda',
                    age: 2022 - 2002,
                    friends: ['John', 'Kelvin', 'Chanda', 'Kabwe']
                        };

                        profileDetails.firstName = 'Collins';

                        console.log(profileDetails);  

                        // console will display 
                                        age: 20
                                        firstName: "Collins"
                                        friends: (4) ['John', 'Kelvin', 'Chanda', 'Kabwe']
                                        lastName: "Banda"   

- Javascript object allows us to get a single element 
- Example: 

                 const profileDetails = {
                    firstName: 'Peter',
                    lastName: 'Banda',
                    age: 2022 - 2002,
                    friends: ['John', 'Kelvin', 'Chanda', 'Kabwe']
                        };

                        console.log(profileDetails.firstName); 

                        // display Peter

- You can access specific data from a JavaScript object  using the  ```Prompt``` method.
- When you enter job in the prompt pop up, the console will display Banker.
- Example:


                   const Petro = {
                    firstName: 'Jonas',
                    lastName: 'Kabwe',
                    age: 2022 - 2001,
                    friends: ['Chanda', 'Kabwe', 'Angela'],
                    job: 'Banker'
                                };

                    const getInformation = prompt('What do you want to know about Petro; job, firstName, lastName, age, or friends?');

                    console.log(Petro[getInformation]);





                            