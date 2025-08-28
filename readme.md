### 6. JavaScript DOM and Event Handling Questions

 Answer the following questions clearly:

1. What is the difference between *getElementById, getElementsByClassName, and querySelector / querySelectorAll*?

Ans:
1.getElementById: Finds one element by its unique ID. Though IDs are special and only used once, it gives just that one element.

2.getElementsByClassName: Finds all elements that have a certain class name. It gives a list of all the elements.

3.querySelector:This finds the first element that matches any CSS selector wanted, like 
-class, 
-ID, 
-tag.

4.querySelectorAll:It finds all the elements that matches the CSS selector and gives a list of them.

2. How do you *create and insert a new element into the DOM*?
Ans:
// Create a new paragraph:-
const newParagraph = document.createElement('p');
newParagraph.textContent = 'Hello! Creating and inserting new element.';

//Insert to the page:-
document.body.appendChild(newParagraph);

3. What is *Event Bubbling* and how does it work?
Ans:
When clicking something inside on the page, the event starts at the thing that was clicked and then moves up to its parents, then their parents, and so on. This is called event bubbling. Means many elements can react to the same click, one after another.

4. What is *Event Delegation* in JavaScript? Why is it useful?
Ans:
Instead of putting event listeners on lots of little elements, put one listener on their parent. When a child element is clicked, the event bubbles up to the parent, and then it can be checked that which child was clicked.It is useful because it is easier and faster because it only need one event listener.
It works later even if new child elements were add on.

5. What is the difference between *preventDefault() and stopPropagation()* methods?
Ans:
1.preventDefault() methods: Stops the browser’s normal action (like opening a link).
2.stopPropagation() methods: Stops the event from moving up to parent elements.