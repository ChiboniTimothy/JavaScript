### DOT NOTATION AND BRACKET NOTATION

- Both Dot and Bracket Notations are used for accessing a property in a JavaScript object

### DOT NOTATION
- We can use Dot notation to grab a property from the object
- Example:

             const profileDetails = {
                    firstName: 'Peter',
                    lastName: 'Banda',
                    age: 2022 - 2002,
                    friends: ['John', 'Kelvin', 'Chanda', 'Kabwe']
                        };

                        console.log(profileDetails.firstName); 

                        // Console will display Peter

### Bracket Notation 
- Bracket Notation can access properties in an object by introducing the brackets
- Example:

             const profileDetails = {
                    firstName: 'Peter',
                    lastName: 'Banda',
                    age: 2022 - 2002,
                    friends: ['John', 'Kelvin', 'Chanda', 'Kabwe']
                        };

                        console.log(profileDetails['firstName']); 
                        
                        //  console will display Peter

- Bracket Notation allow us to put any expressions we feel like in the object unlike Dot Notation will only allows putting a real defined property
- Example:

             const profileDetails = {
                    firstName: 'Peter',
                    lastName: 'Banda',
                    age: 2022 - 2002,
                    friends: ['John', 'Kelvin', 'Chanda', 'Kabwe']
                        };

            const nameKey = 'Name';
                        console.log(profileDetails['first' + nameKey]);

                        //  console will display Peter

- If you use Dot Notation to access a property in an object with a created variable it will display an error in the console.
- There is a limit to which Dot notation can access the property in an object
- Dot notation will only access a real defined property
- Bracket notation is able to access a property in an object with a created variable 
- Example: 

                    const profileDetails = {
                    firstName: 'Peter',
                    lastName: 'Banda',
                    age: 2022 - 2002,
                    friends: ['John', 'Kelvin', 'Chanda', 'Kabwe']
                        };
                    const interestedIn = prompt('Choose between job, firstNmame, lastName, age, friends');

                    console.log(profileDetails[interestedIn])

- If you run this code in a JavaScript file, it will display a pop up and if you enter job, in the console it will display Banker.

        