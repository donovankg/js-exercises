#Javascript Questionnaire

###Javascript General

1. How do you debug web applications?
   *  two main ways. console.log(); in different places of the code to see whats running and what the varaiables are to 
   make the code work. the other way is the use of the developer tools (f12 for windows) and (right click dev tools for 
   mac).
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
  	* it allows you to use parts of one object into another.
15. Explain how the bind function works
    1. If an older browser does not have the bind function, how will you shim it?
	* you would make a prototype of bind to Function. I would refer to the mdn site on how to apply it https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Function/bind
    2. Create an Example
	* 
16. How would you implement currying for any function?
  	*I would pass arg into a function and return them back.
	function test(arg){
		return arg+' said hi.'}
	test('Bob');
17. What is a closure?
  	* They are functions that refer to variables that remember the enveriment that they came from.
18. What is AJAX.
	* its client side script that allows data to be passed from db without a postback.
19. Explain how JS can interact with RESTful APIs.
	* by using curd, create, read, update, , delete.
20. Explain how hoisting works.
	* as the page is loaded, all the declared items are moved to the top in memory so they can be put into memory first.
21. What are the different way of accessing an object's properties? Explain the difference.
	* for(key in Obj){
	     obj[key]	
	  }
	  this will allow you to access each of the perporties.
22. How would you compare two objects in JavaScript?
	* I'd use object.is(). you place the two objs in and it would return true or false.
23. What is the this keyword?
	* this refers to the enverienment that it was created in.
24. What are event bubbling and capturing?
	* bubbling is when you a child is the target but if you click the parent then it would be targeted as well. capturing is the reverse; the parent has an event or something and the child also has it because of inharatance.
25. What does mean event delegation? How to use it?
	* it allows you to use one function for many events. it prevents there from having many functions that all do the same thing.
26. How can event propagation be stopped?
	* Event.stopPropagation() will allow it the be stopped.
27. How can event default behavior be prevented?
	* by setting up function that uses event.preventDefault(). it stops whatever event that triggers this function.
28. Explain the use of timers. Name some of their drawbacks.
	* it allows you to semiulate loading in the app; you can have a single delay, intervals, and imdedate.
	draw backs are that you have to wait for them to complete or you may miss that its there if the timer is off.
29. What is the difference between function declaration and function expression?
	* declaration is anything that has a var in front of it or an IIFE. delcarations get hosted while the other does 	   not.
30. What is an Immediately-Invoked Function Expression (IIFE)?
	* because js is single thread, when it comes and sees the iife, it is ran right then rather than waiting.
31. What is the default value of javascript variables?
	* undefined
32. What happens if there is no return statement in a function?
	* no values are returned, you can change variables that are outside that function, log things out, or run
	other functions though.
32. How do you add items to the DOM using JavaScript?
	* Object.create
33. If there are two elements with the same id, which element will be returned by getElementById()?
	* The first will be returned but its very bad practice to use an ID more than once.
34. What are DocumentFragments?
	* It allows you to put parts of your pages into modules allowing you to use them more than once.

###Patterns 

1.	What is a singleton and how do you create one in JavaScript?
	* it makes it so that if you call a function many times you will still only get the same value or results.
2.	What is the module pattern and how do you apply it?
	*	module patterns allow you to have private variables so that you don't pollute the global scope.
3.	What is the revealing pattern?
	*	it displays hidden information in the javascript.
4.	What is the facade pattern?
	*	its an object that makes it easy to use the data inside it.
5.	What is the factory pattern?
	*	this pattern allows you create new objects.

###Best Practices

1.	Explain the effect of 'use strict'?
	* 	it helps prevent errors and makes the site more safe.
2.	What are some ways of improving performance in JavaScript?
	*	avoid using repeated code, have it be reusable.
3.	Mention a few JS OOP best practices.
	*	use design patterns, don't polute the globel scope, make reusable code.
4.	What is unobtrusive javascript?
	*	its the seperation of the javascript from the html code.
5.	List 5 good and 5 bad practices of JavaScript
	  * good: use wrapper functions, leave comments in your code, use returns, use patterns, use libereries that are 
	  aviable.
	  * bad: leaving console.log in, poluting the global scope, using too many divs, not using dynamic elements, not 
	  backing up your work on a repo.
6.	What is the same origin policy?
		*	it allows the scripts to be used in multiple pages as long as they come from the same origin.
7.	Explain how thread safety works in JavaScript
		*	there is normally no issues, because JS is single threaded, one thread finishs before another begins.
