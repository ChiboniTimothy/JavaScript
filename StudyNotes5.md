## JAVASCRIPT CONTINUATION

- Before writing any code in a ```script.js```  file, write ```'use strict';```.
- ```'use strict';``` enables the environment to specifically show visible errors in the code.
- When you write a code with a mistake, ```'use strict';``` will expose that error
- Example:

                let hasDriversLicense = false;
                const passTest = true;

                if(passTest)hasDriverLicense = true;
                if(hasDriverLicense) console.log('I can drive');

- The code above will not display because it has an error, so ```'use strict';``` will specifically show the error causing the code not to work.

### CONTINUATION OF FUCNTIONS

- Parameters are like variables which are specific to a function and they can only be defined when the function is called or invoked.
- When you define your function, you add params which let us know that the function expects to be passed some data.
- Example:

                    // Oranges and Mango are parameters of the JuiceMaking function

                function juiceMaking(Oranges, Mango){  
                    // Body of the function
                    const OrderMaking = ` I want cake with ${Oranges} Oranges and ${Mango} Mango.`;

                        // Return in the function enables us to return a speficied value from the function.

                        return OrderMaking;
                }
                    // Calling the function and having the parameters defined

                    console.log(juiceMaking(4, 5));

- Functions can be reused over and over again.
- Example:
                // We are reusing the function above

                const niceJuice = juiceMaking(3, 0)
                console.log(niceJuice);

- Function can also be returned like

                        function calcAge_1(birthYear){
                            return 2022- birthYear;
                        }

                        console.log(calcAge_1(2002));

- Function can also be written without a name and these functions are called ```Anonymous Function```.
- Example:

                const calcAge_2 = function (birthYear){
                    return 2022 - birthYear;
                }

                const age = calcAge_2(2002);
                console.log(age);

- Arrow function is simply a form of function expression and it's shoter and faster to write.
- Example:

                const fruitProduction = mango => `I am only interested in eating health food like salads with ${mango} mangos`;

                 const fruitMarket = fruitProduction(4);

                 console.log(fruitMarket);

- When you have a single variable in the body of the function when using the arrow function, return is automatically initiated.
- When you have more than one variable in the body of the function when you are using the arrow function return and the curl brackets should be included in the body.
- Example:

                const retirementAge = birthYear => {
                const age = 2022 - birthYear;
                const retirement = 65 - age;
                return retirement;
                }

                console.log(retirementAge(1990));