### MANIPULATING CSS STYLES

-JavaScript gives us the ability to apply CSS styles to a single or group of DOM components, edit or remove them, or even change the entire stylesheet for the entire page.
- Accessing the "HTML" element is always the best course of action when manipulating "CSS" with JavaScript.
- For instance, if we want to modify the styles of our element in response to a button click, we must first listen to the click event and then attach a function with the preceding code.
- Example 1:

            const button = document.querySelector('button');
            button.addEventListener('click', () => {
                const element = document.querySelector('.demo');
                element.style.backgroundColor = 'red';
                });

- Example 2:

                document.querySelector('body').style.backgroundColor = 'white';

- In the above example, we are accessing the "'body"' tag in HTML and styling it with CSS.
- JavaScript can be used to style CSS as well.

            document.querySelector('.class name').style.width = '23rem';

### REFACTORING CODES IN JAVASCRIPT

- Refactoring in JavaScript is the process of changing a piece of code without changing how it functions. In other words, you can change the internal structure of a particular function, class, module, etc. without modifying the results. Writing clear, understandable, and maintainable code is the foundation of refactoring. It involves writing insightful comments, error messages, adhering to norms like naming conventions, code organization, and modularizing large sections of code and knowing how to structure those modules.


### MODAL WINDOW PROJECT

- This is project focused on adding, removing hidden classes using JavaScript
- In HTML, you can use the same class for different buttons and these class can be selected by ```document.querySelectorAll()``` this DOM allows us to see all the name of same classes 

                <button class="show-modal">Click Modal 1</button>
                <button class="show-modal">Click Modal 2</button>
                <button class="show-modal">Click Modal 3</button>

- ```document.querySelectorAll()``` allows to loop through the classes of the button and we can add the ```addEventListener```.
- For example: 

for(let i = 0; i < openModal.length; i++){
    openModal[i].addEventListener('click', function(){

    })
}
- We can now use the ```classList``` property to display the modal with a hidden class.
- A ```classList``` property allows us to add the ```remove``` method to remove muitiple classes by passing the command line like

        modal.classList.remove('hidden');

- We do not use a ```.hidden``` when removing a hidden class in this case, we just write ```'hidden'```
- Classes are like containers with a lot of properties in them.

 ### Handling an Escape Key Press Event 

 - Keyboard events are listened on all the document. 
 - For example: 

                document.addEventListener('keydown/up/press', )

- ```Keyup``` only happens when we lift our finger off the keyboard or key
- ```keydown``` only happens when we press down a key. However, when a keydown event occurs, Javascript usually generates an object which contains all the information about an event and we can access the information.
-  ```keypress``` is fired continous as we keep our fingers on the key

- If we pass a paramenter, we will be able to see the key which was pressed on the keyboard
- For example: 

                document.addEventListener('keyydown', function(e){
                    console.log(e.key) // enables us to see the key pressed on the keyboard 
                })


### ClassList Property

- The ```classList``` property is used to represent the value of the class elements, which is a DOMTokenList object. It is a read-only property, but we can change its value by modifying the classes used in the program. The JavaScript classList property includes the following methods for performing various operations on class elements:

1. ```add()``` method is used for adding one or more classes to the element.
2. ```remove()``` method is used for removing one or more classes from the number of classes present in the element.
3. ```toggle()``` method is used for toggling the specified class names of an element. It means on one click the specified class gets added and on another click the class gets removed. It is known as the toggle property of an element.
4. ```replace()``` method is used for replacing an existing class with a new class.
5. ```contains()``` method of the JavaScript classList property is used for returning the Boolean value as an output. If the class exists, the value is returned as true; otherwise, it is returned as false.
6. ```item()``` method is used for displaying the name of the classes at the particular index. Thus, it returns the class name.

- To add an ```ID``` and the defined variable, we can write as 

            let playing = 0;
            document.getElementById(`id name${playing}).textContent = 2;
- We can select an ```ID``` by either:

        document.getElementById('ID name');

        or 

        document.querySelector('#ID name');

- 