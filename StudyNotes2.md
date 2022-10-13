## JAVASCRIPT OPERSTORS

- JavaScript includes operators same as other languages. 
- An operator performs some operation on single or multiple operands (data value) and produces a result. 
- For example, in 1 + 2, the + sign is an operator and 1 is left side operand and 2 is right side operand. 
- The + operator performs the addition of two numeric values and returns a result.

## CATEGORIES OF JAVASCRIPT OPERATORS

- JavaScript includes following categories of operators.

 ### Arithmetic operators

 - Arithmetic operators are used to perform mathematical operations between numeric operands. e.g ```+ (addition)``` adds two operands A + B  ```- (subtraction)``` subtracts the operand from the first A - B etc

### Comparison operators

- JavaScript provides comparison operators that compare two operands and return a boolean value ```true``` or ```false```.

- ```==``` - Compares the equality of two operands without considering type.
- ```===``` - Compares equality of two operands whilr considering type.
- ```!=``` - Compares inequality of two operands.
- ```>``` - Returns a boolean value true if the left-side value is greater than the right-side value; otherwise, returns false.
- ```<``` - Returns a boolean value true if the left-side value is less than the right-side value; otherwise, returns false.
- ```>=``` - Returns a boolean value true if the left-side value is greater than or equal to the right-side value; otherwise, returns false.
- ```<=``` - Returns a boolean value true if the left-side value is less than or equal to the right-side value; otherwise, returns false.
- Example: 

     JavaScript Comparison Operators

               var a = 5, b = 10, c = "5";
               var x = a;

               a == c; // returns true

               a === c; // returns false

               a == x; // returns true

               a != b; // returns true

               a > b; // returns false

               a < b; // returns true

               a >= b; // returns false

               a <= b; // returns true

### Logical operators

- Logical operators are used to combine two or more conditions. 
- JavaScript provides the following logical operators.

- ```&&``` is known as AND operator.
- It checks whether two operands are non-zero or not (0, false, undefined, null or "" are considered as zero). 
- ```||``` is known as OR operator. 
- It checks whether any one of the two operands is non-zero or not (0, false, undefined, null or "" is considered as zero). 
- ```!``` is known as NOT operator. 
- It reverses the boolean result of the operand (or condition).
- Example: 
           
            Logical Operators

                        var a = 5, b = 10;

                        (a != b) && (a < b); // returns true

                        (a > b) || (a == b); // returns false

                        (a < b) || (a == b); // returns true

                        !(a < b); // returns false

                        !(a > b); // returns true

### Assignment operators

- JavaScript provides the assignment operators to assign values to variables with less key strokes.

- ```=``` - Assigns right operand value to the left operand.
- ```+=``` - Sums up left and right operand values and assigns the result to the left operand.
- ```-=``` - Subtract right operand value from the left operand value and assigns the result to the left operand.
- ```*=``` - Multiply left and right operand values and assigns the result to the left operand.
- ```/=``` - Divide left operand value by right operand value and assign the result to the left operand.
- ```%=``` - Get the modulus of left operand divide by right operand and assign resulted modulus to the left operand.

- Example: 
 
           Assignment operators

                                var x = 5, y = 10, z = 15;

                                x = y; //x would be 10

                                x += 1; //x would be 6

                                x -= 1; //x would be 4

                                x *= 5; //x would be 25

                                x /= 5; //x would be 1

                                x %= 2; //x would be 1

### JavaScript if-else Condition

- JavaScript includes if-else conditional statements to control the program flow.
- JavaScript includes following forms of if-else conditions:
  - if condition
  - if-else condition
  - else if condition
  - if condition
- Use if conditional statement if you want to execute something based on some condition.
- Example: 
 
              if condition

                        if( 1 > 0)
                        {
                            alert("1 is greater than 0");
                        }

                        if( 1 < 0)
                        {
                            alert("1 is less than 0");
                        }
                
- The above example clearly tells that the first if statement contains 1 > 0 as conditional expression. - The conditional expression 1 > 0 will be evaluated to true, so an alert message "1 is greater than 0" will be displayed, whereas conditional expression in second if statement will be evaluated to false, so "1 is less than 0" alert message will not be displayed.

### else condition

- Use else statement when you want to execute the code every time when if condition evaluates to false.
- The else statement must follow if or else if statement.
- Example: 

                else condition

                    var age = 50;
                    var yourAge = 100;

                    if( age > yourAge)
                    {
                        alert("My age is greater than yourAge");
                    }
                    else
                    {
                        alert("My age is less than or equal to yourAge");
                    }

- JavaScript allows multiple else if statements also.
- Example: 

                Multiple if else conditions

                var age = 500;
                var yourAge = 1000;

                if( age > yourAge)
                {
                    alert("My age is greater than yourAge");
                }
                else if(age < yourAge)
                {
                    alert("My age is less than yourAge");
                }
                else if(age == yourAge)
                {
                    alert("My age is equal to yourAge");
                }