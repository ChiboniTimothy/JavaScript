# JavaScript Sets

- A set is a collection of unique values meaning that a set can never have duplicates
- To create a set we need to write ```new set()``` then pass in inputs
- Example: 

           const arr = [new Set([2, 3, 4, 5, 5])];
            console.log(...arr);

- Getting the ```size``` of a set, we write as 

            const arr = [new Set([2, 3, 4, 5, 5]).size];
            console.log(...arr);

- You can check if a certain  element is in a set by writing 

            const arr = [2, 3, 4, 5, 5];
            const arr1 = new Set(arr.has(name of the element))
            console.log(arr1);

- You can add an element to a set by writing 
            const arr = [2, 3, 4, 5, 5];
            const arr1 = new Set(arr.add(name of the element))
            console.log(arr1);

- You can also delete an element in a set like

            const arr = [2, 3, 4, 5, 5];
            const arr1 = new Set(arr.delete(name of the element))
            console.log(arr1);

- You can clear all the elements inside a set 

            const arr = [2, 3, 4, 5, 5];
            const arr1 = new Set(arr.clear(name of the element))
            console.log(arr1);

- However, you can loop through a set like
            for(const order of arr1)
            console.log(order);

## JavaScript Maps

- A map is a data structure that we can use to map vales to keys.
- To write a ```Map``` You first need to create an empty map by writing 

            const rest = new Map();
            rest.Set('Name', 'Timothy');
            console.log(rest)

                    OR

            const rest = new Set([
                ['Question', 'What is your name?'],
                ['location', 'Zambia'],
                ['Continent', 'Africa']
            ])
            console.log(rest)