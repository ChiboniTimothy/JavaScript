
### DOCUMENT OBJECT MODEL (DOM)

- You can access a text between two HTML  tags using the JavaScript keyword ```textContent```
- For example:

           document.querySelector('.name of class').textContent;

- DOM allows Javascript to access HTML elements and styles to manipulate them.
- ```document``` is the special object that is the entry point to the DOM
- For example:

               document.querySelector()

### HANDLING CLICK EVENTS

- Event is something which happens on the page e.g moving a mouse, mouse click, key clicker
- Event listener helps us to wait for certain events to happen then react to them.
- Javascript method ```Math``` is an object that JavaScript gives and in the ```Math``` method there are different kinds of objects.
- ```random``` is one of the ```Math``` object which gives numbers between ```0``` and ```1```.Whenever, we run ```Math.random``` it will always give a different number. If we want to get numbers between 0 and 20 then we need to multiply ```Math.random * 20``` and to remove decimals we use ```Math.trunc(Math.random * 20) + 1```.

### MANIPULATING CSS STYLES

- When we want to manipulate  ```CSS```, we should always try to access the element we want to manipulate by writing 

                    document.querySelector('body').style.color