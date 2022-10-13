### OBJECT METHODS

- Object methods are able to hold different types of data including functions, arrays, and boolens etc
- Object methods can also hold objects inside them 
- Example: 

                const profileDetails = {
                    firstName: 'Timothy',
                    lastName: 'Chiboni',
                    birthYear: 2000,
                    job: 'Data Analyst',
                    hasDriversLicense: true,
                    calAge: function(birthYear){
                        return 2022 - birthYear;
                    }
                };
- Accessing the property ```calAge```

                    // Dot Notation
                console.log(profileDetails.calAge(2000)) 

                // Bracket Notation
                console.log(profileDetails['calAge'](2000));

- However, you can access the property ```calAge``` without passing a parameter in the function and console by using a JavaScript keyword called ```this```
- The keyword ```this```  is basically equal to the object calling the method
- Example:

            const profileDetails = {
                    firstName: 'Timothy',
                    lastName: 'Chiboni',
                    birthYear: 2000,
                    job: 'Data Analyst',
                    hasDriversLicense: true,
                    calAge: function(){
                        return 2022 - this.birthYear;
                    }
                };

                console.log(profileDetails.calAge())

                // console will display 22

- The keyword ```this``` can also be used to add a new property and value.
- Example:

             const profileDetails = {
                    firstName: 'Timothy',
                    lastName: 'Chiboni',
                    birthYear: 2000,
                    job: 'Data Analyst',
                    hasDriversLicense: true,
                    calAge: function(){
                        this.age = 2022 - this.birthYear;
                        return this.age;
                    }
                };

                    console.log(profileDetails['calAge]());

- To access the boolean using the keyword ```this```
- The boolen property has value false meaning that it will display ```no``` but when the property is set to true it will display ```a```
- Example:

                const profileDetails = {
                    firstName: 'Timothy',
                    lastName: 'Chiboni',
                    birthYear: 2000,
                    job: 'Data Analyst',
                    hasDriversLicense: false,
                    calAge: function(){
                        this.age = 2022 - this.birthYear;
                        return this.age},
                    getSummary: function(){
                        return `${this.firstName} has a ${profileDetails.calAge()} years old, who has ${this.hasDriversLicense? 'a' : 'no'} driver's license`
                    }
                    }

                     console.log(profileDetails.getSummary());

### ITERATION: THE FOR LOOP
- Loops are fundamental aspect of every programming language
- Loops allows to automate repetitive tasks that will need to perform over and over
- The ```for loop``` has three parts
- First part is the initial value of a counter
- Counter is the value starting from 1 to 10 e.g ``` for(let i=1)```
- The second part of the ```for loop``` is the logical condition that is evaluated before each iteration ends the loop
- Example ``` for(let i=1; i <= 10;)```
- The third part of the ```for loop``` updates the counter each time the iteration loops through
- Example ```for (let i=1; i<=10; i++)
- Executing the ```for loop```
- Example:

            for(let i=1; i<=10; i++){
                console.log('Gym time Chiboni')
            }
                // console will display 10 Gym time Chiboni

- To display multiple loops in console create the template in the console and call the variable ```i```
- Example: 

                for(let i=1; i<=10; i++){
                    console.log(`Gyme time Chiboni ${i}`)
                }
                   
