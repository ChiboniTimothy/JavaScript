### LOOPING ARRAYS

- ```for loops``` can also be used to loop through an array
- Example:

                const profileInfo = ['Jonas', 'Chanda', 'Mando', 2000];
                for (let i = 0; i < 5; i++){
                    console.log(profileInfo[i]);
                };

- To make the code more efficiency, there is need to compute the code than hand coding it like i did in the previous example using ```i < 5``` 
- Instead of hand code, you can just use ```i = profileInfo.length``` which makes it easy and accurate
- Example: 

               const profileInfo = ['Jonas', 'Chanda', 'Mando', 2000];
                for (let i = 0; i < profileInfo.length; i++){
                    console.log(profileInfo[i]);
                };

### FILLING EMPTY ARRAYS USING FOR LOOPS

- Filling an empty array with elements, you first need to create an array and elements in it then another empty array
- An empty array looks like this ```[]```
- There are two ways of filling up empty arrays, both will be showed below
- Example: 

            const years = [2000, 2001, 2002, 2003, 2004];
            const ages = [];

            for(let i=0; i = years.length; i++){
                ages[i] = 2022 - years[i];
            }
            console.log(ages);

            OR

- You can also use the ```push method``` to fill an empty array

            const years = [2000, 2001, 2002, 2003, 2004];
            const ages = [];

            for(let i=0; i = years.length; i++){
                ages.push(2022 - years[i]);
            }
            console.log(ages);

### THE CONTINUE AND BREAK LOOPS

- The continue statement is used to exit the correct iteration of the loop and continue to the next one 
- ```continue loop```  skips a non string and only executes strings
- Example: 

             const years = [2000, 'Home', 2001, 'Hello', 2002, 'Welcome, 2003, 2004];
             for(let i = 0; i = years.length;){
                 if(years[i] !== 'string') continue;

                 console.log(years[i], typeOf years[i]);
             }

             // only Home, Hello and Welcome will be executed and numbers will be skipped

- ```break loop``` is used to completely terminate the whole lopp execution.
- When the ```break loop``` is runs it finds that there is numbers and strings mixed the loop iteration will be completely terminated without displaying anything in the console
- Example:

            const years = [2000, 'Home', 2001, 'Hello', 2002, 'Welcome, 2003, 2004];
            for(let i = 0; i = years.length; i++){
                if(years[i] === 'numbers')break;
                console.log(years[i], typeOf years[i]);
            };