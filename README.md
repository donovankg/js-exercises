# Javascript-docs

##Javascript basic

1. [MDN Javascript Introduction](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript#Objects)
2. [Tutorial Control Flow](https://www.codecademy.com/courses/javascript-beginner-en-qDwp0/0/1) 
3. [Array Doc](https://github.com/KsquareLabs/javascript-intro-to-arrays)
4. [Object Doc](https://github.com/KsquareLabs/javascript-objects)


##Exercises

###Chapter 3.

1. Create a function that will multiply two numbers. The function must return the result in base 13. 

    Example: 
    ```javascript
    var answer = mul (9, 6); // 42 
    ```
    Basic function creation together with built­in JS Math functionality. 

2. Create a function that will return the addition of N numbers. 

    Example: 
    ```javascript
    var answer = add (1, 2) + add ( 1, 4, 6, 7, 2); 
    ```
    Dynamic argument list handling with JS 

3. Create an object that will hold methods for adding, multiplying, and factorial operations. 

    Example: 
    ```javascript
    var a = myMath.add (1, 2, 3); //6 var b = myMath.mul (1, 2, 3); // 6 
    
    var c = myMath.fact ( 3); // 6 
    ```
    
    Use of anonymous functions and functions as object properties (methods.)  


4. Create a custom object that will hold an image’s mock information such as pixel color                             data, image size, and name. It must be able to return the information. 

    Example:
    ```javascript
    var data = new Array (1600); // 40 x 40 px dummy image data 
    var img = new Image (data, 40, 40, ‘myImage’); 
    img.width; // 40 
    img.height; // 40 
    img.name; // ‘myImage’ 
    
    img.pixelData (20, 4); // returns the color of the pixel at that position. 
    ```

5. Create a function that will print out the properties of an object.  

    a. If one parameter is provided, it should print out all of the properties accessible by that object. 
    
    b. If a second, boolean value, parameter is provided, it should only print out the values that belong to the object instance itself if true.  

  Example: 
  ```javascript
  function CustomObject (a, b) { 
    this.a = a; 
    this.b = b; 
  } 
  CustomObject.prototype.c = function () { return this.a + this.b; }; 
  var obj = new CustomObject (1, 2); 
  printObjProp (obj); // output: a, b, c
  printObjProp (obj, false); // output: a, b, c 
  printObjProp (obj, true); // output: a, b 
  ```

###Chapter 4

1. Create a recursive function that will calculate the fibonacci value of a number. 

    Example: 
    ```javascript
    var n = fibonacci (4); // 3 var m = fibonacci (9); // 34 
    ```
    Use of recursion. 

2. Create a function that will recursively go through all of the elements of an array of                               numbers and add them. 

    Example: 
    ```javascript
    var arr = [ 1, 3, 5, 7]; var sum = addRec (arr); // 16 
    ```
    Use of recursion. 

3. Create a custom object type that will hold a number value.  

    a. Make sure that no other data type can be assigned to that variable.  
    
    b. It must hold ONLY numbers.  
    
    Validation, setters & getters, private variables 

4. Write a function that will accept any number of arguments and print out their data type. 

    Example: 
    ```javascript
    dataType (1, 6.2831, “pi*2”, [function(){}, 1], {}, function () {});  // number, float, string, array, object, function 
    ```
    
    Variable argument functions & data types 

5. Write a function that will calculate the distance between two points. The function should                           be able to handle 2D and 3D points. 

    Example: 
    ```javascript
    var x1 = 1, y1 = 2, z1 = 1; 
    var x2 = 2, y2 = 2, z2 = 4; 
    var delta1 = distance (x1, y1, x2, y2); // delta = 1 var delta2 = distance (x1, y1, z1, x2, y2, z2); // delta = 3.1622… 
    distance (x1, x2); // should throw an error: Insufficient parameters 
    ```
    Function overloading and validation

6. Make the function from exercise 5 accept its parameters as either a parameter list or as                               two arrays containing 2D or 3D point data.  

    Example: 
    ```javascript
    distance (1, 2, 2, 2); // returns 1 (done as part of exercise 5) distance ([1,2], [2,2]); // returns 1 
    distance ([1,2], [2,2,4]); // error: incompatible point data 
    ```
    
    Function overloading and validation 

##Resources

1. Eloquent JavaScript Book (1-4).
2. Secrets of the JavaScript Ninja.

