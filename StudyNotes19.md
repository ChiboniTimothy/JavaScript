### Spread Operators(...)

- Spread syntax (...) allows an iterable, such as an array or string, to be expanded where there are zero or more arguments (for function calls) or elements (for array literals). The spread syntax in an object literal enumerates an object's properties and adds key-value pairs to the object being created.
- Example :

                const arr = [1, 2, 3, 4];
                const copyArr = [...arr];
                console.log(copyArr)

### Rest Pattern and Parameter

- The rest parameter syntax allows a function to accept an indefinite number of arguments as an array, allowing variadic functions to be represented in JavaScript.
- Rest pattern is always found on the left side of an arry or object.
- Example :

                const arr = [2, 3, 4, 5];
                const [a, ...others] = arr;
                console.log(a, others);
- ```others``` means creating a  new  array inside an array

- Rest Parameter allows a function to accept an indefinite number of arguments as an array
- Example: 

                function parameterRest(obj){
                    console.log(obj)
                }

                parameterRest({
                    name: 'Peter'
                })

### Short Circuiting (&& and ||)

- In JavaScript, short-circuiting is the evaluation of an expression from left to right with ```||``` and ```&&``` operators.
- Example: 

            console.log(0 || 'String')

- If the first value is not true, Javascript will not even evaluate but instead it will execute the alternative value. In the example above ```0``` is undefined so Javascript will execute ```string```

- The && operator will return false as soon as it gets any falsy value and will return the last true value if all the values are truthy.
- Example : 

                console.log('' && 'string)

- The execution stops immediately Javascript finds a false value and it will not execute an alternative value 


### Optional chaining (?.)

- Optional chaining help access an object's property or calls a function. If the object is undefined, null it returns undefined instead of throwing an error

### Looping objects: Object keys, values and entries

- ```object.keys()``` returns an array iterator object with the keys of an object.
- Example: 

                const proprty ={
                    town: 'Lusaka',
                    country: 'Zambia',
                    year: '2022'
                }

                const arr = object.keys(property)
                console.log(arr);

- ```object.values()``` returns an array iterator object with the values of an object
- Example: 

                 const proprty ={
                    town: 'Lusaka',
                    country: 'Zambia',
                    year: '2022'
                }

                const arr = object.values(property)
                console.log(arr);

- ```object.entries()``` returns everythingincluding index, keys and values of an object.
- Example:

                 const proprty ={
                    town: 'Lusaka',
                    country: 'Zambia',
                    year: '2022'
                }

                const arr = object.entries(property)
                console.log(arr);

- If we want to get the element  in an array using the ```object.entries()``` method we write name of an array.entries
- Example: 

                const game = [2, 3, 4, 5];
                console.log(game.entries());

- If we want to get the elements of object write ```object.entries(name of an object)```
- Example: 

                    const proprty ={
                    town: 'Lusaka',
                    country: 'Zambia',
                    year: '2022'
                    }

                const arr = object.entries(property)
                console.log(arr);

            

