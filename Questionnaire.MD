#Javascript Questionnaire

###Javascript General

1. How do you debug web applications?
   *  two main ways. console.log(); in different places of the code to see whats running and what the varaiables are to make the code         work. the other way is the use of the developer tools (f12 for windows) and (right click dev tools for mac).
2. Explain OOP concepts used in JavaScript?
    * Object-oriented programming. Javascript simulators true OOP from other languages like java, C etc. JS takes name spaces and applies properties (variables, methods, functions) to them. 
3. Can inheritance be done without using prototype? Explain your answer.
    * javascript requires prototypes to do inheritance because it properties from one object to another.
4. Explain the use of a hash-map in JS.
    * hash maping allows you to add properties into a object very easily. if you have an object (var pets = {}) then you would be able to add them like so, pets.dog = {name="bob", age: 5}. then if you wanted to print all of animal you could console.log(animal) or do (animal.dog) to get just the information you just entered.
5. Explain the use of arrays in JS.
  * arrays, as in any langauge, are able to store limitless amount of data into a single variable. 
6. Explain the use of the following methods
    1. Array.prototype.some() 
	* it will check to see if at least one of the args returns back true.
    2. Array.prototype.reduce() 
	* it allows the callback to hold the current and previous values.
    3. Array.prototype.every() 
      * checks everything in an array for the values to be true else returns back false if any of them are false.
    4. Array.prototype.map() 
      * takes the arg and allows you to callback each element in an array.
7. What is an object literal?
	* its simply an object that has everything separated by commas in a list.
	```Javascript
	Var cat = {
		Feet: 4,
		Talks : ‘meow’,
		Fleas: true
};
```
8. Explain how string types work. How can you manipulate a string efficiently?
	* a variable that has “ sample” will be set as a string. It can be manipulated by dot notation. Examples would be as 
	follows:
	```javascript
	var txt = 'this is a test';
	console.log(txt);
	console.log(txt.length);
	console.log(txt.indexOf('test'));
	```
9. What is the difference between 1 == "1" and 1 === "1" .
    * the first will return true, the 2nd false. the first looks to see if the character’s match and JS will covert it from number to 
      string and back, the 2nd checks to see if they are a match not only in character but in type as well (string, int, etc).
10. Explain the use of the var keyword. What happens if it is not used?
	* var makes characters into a variable. Most of the times it will return something as undefined.  Even when it doesn’t it’s still best practice to define things as a variable. 
11. Explain the next object methods
    1. Object.freeze
    	* a method that stops new properties from being added to the object.
    2. Object.seal
    	* a method that stops new properties from being added and makes existing properties non-configurable.
    3. Object.defineProperty
    	* defines a new property that’s directly on an object or modifies an existing property on an object and returns it.
    4. Object.create
    	* makes a new object with a specified prototype  and properties.
11. When should you return null and when should you return undefined?
  	* you shouldn’t use null. It’s a bad habit. 
12. Is JavaScript pass by reference or pass by value?
  	* By value.
13. If you want to use an arbitrary object as the value of this, how would you do that?
  	* you would need to first use the function.prototype.bind function method, it would take the arbitrary object as its first argument and it would serve as ‘this’ for the function call.
14. Explain the use of call and apply.
  	* 
15. Explain how the bind function works
    1. If an older browser does not have the bind function, how will you shim it?
	*
    2. Create an Example
	*
16. How would you implement currying for any function?
  	*
17. What is a closure?
  	* 
18. What is AJAX.
	*
19. Explain how JS can interact with RESTful APIs.
	*
20. Explain how hoisting works.
	*
21. What are the different way of accessing an object's properties? Explain the difference.
	*
22. How would you compare two objects in JavaScript?
	*
23. What is the this keyword?
	*
24. What are event bubbling and capturing?
	*
25. What does mean event delegation? How to use it?
	*
26. How can event propagation be stopped?
	*
27. How can event default behavior be prevented?
	*
28. Explain the use of timers. Name some of their drawbacks.
	*
29. What is the difference between function declaration and function expression?
	*
30. What is an Immediately-Invoked Function Expression (IIFE)?
	*
31. What is the default value of javascript variables?
	*
32. What happens if there is no return statement in a function?
	*
32. How do you add items to the DOM using JavaScript?
	*
33. If there are two elements with the same id, which element will be returned by getElementById()?
	*
34. What are DocumentFragments?
	*

###Patterns 

1.	What is a singleton and how do you create one in JavaScript?
	*
2.	What is the module pattern and how do you apply it?
	*	
3.	What is the revealing pattern?
	*	
4.	What is the facade pattern?
	*	
5.	What is the factory pattern?
	*	

###Best Practices

1.	Explain the effect of 'use strict'?
	* 	
2.	What are some ways of improving performance in JavaScript?
	*	
3.	Mention a few JS OOP best practices.
	*	
4.	What is unobtrusive javascript?
	*	
5.	List 5 good and 5 bad practices of JavaScript
	*	
6.	What is the same origin policy?
	*	
7.	Explain how thread safety works in JavaScript
	*	
