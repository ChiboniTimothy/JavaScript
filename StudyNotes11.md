### LOOPING BACKWARDS

- There are several methods to loop through the array in JavaScript in the reverse direction:
1. Using reverse for-loop
- The standard approach is to loop backward using a for-loop starting from the end of the array towards the beginning of the array.
- Example: 


        Const tecNumber = [1, 2, 3, 4, 5];
 
        for (let i = techNumber.length - 1; i >= 0; i--) {
        console.log(techNumber[i]);
        }

2. Using Array.prototype.reverse() function

- The forEach method goes through the array in the forward direction. 
- To loop through an array backward using the forEach method, there is need to reverse the array. 
- We can avoid modifying the original array, first by creating a copy of the array, reverse the copy, and then use forEach on it. 
- Example:


                const techNumber = [1, 2, 3, 4, 5];
                
                techNumber.slice().reverse()
                    .forEach(function(item) {
                            console.log(item);
                        });

- We can alternatively use the Object.keys() method to get keys:

                const techNumber = [1, 2, 3, 4, 5];
                
                Object.keys(techNumber).reverse()
                        .forEach(function(index) {
                            console.log(arr[index]);
                        });

3. Using Array.prototype.reduceRight() function

- The reduceRight() method executes the callback function once for each element present in the array, from right-to-left. 
- Example:

                const techNumber = [1, 2, 3, 4, 5];
                
                techNumber.reduceRight((_, item) => console.log(item), null);

