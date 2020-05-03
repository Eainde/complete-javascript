## THE DOCUMENT OBJECT MODEL

- It is a structered representation of an HTML document.
- The DOM is used to connect webpages to scripts like javascript.
- For each HTML box, there isan object in the DOM that we can access and interact with.

 
####  Math.random()
- it gives a random number between 0 & 1.
#### Math.floor(4.6) // 4
This methods rounds up the floating value.

## document object
- This is the object that will gives the access to DOM.

### document.querySelector('#id')
- This methods is used to select elements from HTML.
- The Document method querySelector() returns the first Element within the document that matches the specified selector, or group of selectors. If no matches are found, null is returned.
- We can also use this method to read the value of the selected element.
    - var x = document.querySelector('#score-0').textContent;
- We can also use this method to change the css.
    - document.querySelector('.dice').style.{css property}
    - document.querySelector('.dice').style.display= 'none';
    
#### document.querySelector('selector').textContent()
- If you want to change the content of the selector element then you can use this mehtod.
    - document.querySelector('#current-' + activePlayer).textContent = '33';
#### document.querySelector('selector').innerHtml()
- If you want to put some HTML in the slected element then you can go for this method.
    - document.querySelector('#current-' + activePlayer).innerHTML = '<em>' + dice + '</em>';
#### document.querySelector('.id/#class').classList.add('css className');
- This method is used to add css class
#### document.querySelector('.id/#class').classList.remove('css className');
- This method is used to remove css class

#### document.querySelector('.id/#class').classList.toggle('css className');
- This method removes the css class if it is there and add a class if it is not there.


### document.getElementById()
- this method is faster than querySelector method and we can use this for id's only.


## Events
- Notifications that are sent to notify the code that something happened on the webpage.

### How events are processed?
- The event can only be processed or handled  as soon as execution stack is empty. Which means all the functions have returned.
- Beside the execution context we also have the message queue in the javascript engine. This is where all the events happen in the browser are put and they sit there waiting to be processed, which only haoppens when execution context stack is empty.
- Event listener is a function which reacts to an event. Since it is a function it gets its own execution context. Which is then put on the top of stack and becomes the active execution context. This is  how the events are processed and how event listener works.
    - document.querySelector('.btn-roll').addEventListener('click', function );
    
- _***Callback Functions:***_ Callback functions are the functions which is called by other functions, and you will only write the name of the function without parentheses() as we did above. 
- _***Anonymous Function:***_ Anonymous functions are the functions which does not have a name, so it cannot be  reused.
