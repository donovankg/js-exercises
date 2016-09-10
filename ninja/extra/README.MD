1. Given an array of words, write a function that will sort the array in ascending order. It should also take an optional argument that can customize the sorting order. Custom sorting orders: 
  1. descending 
  2. sort by length ascending/descending 
  3. sort by number of consonants ascending/descending.  

2. Create a function that can limit the execution of other functions to a determined amount of times.  

 Example: 

  ```javascript
  function limitFunc (fn, num) { ... } 
  var limited = limitFunc (fn, 2); 
  limited ();​
  // executes fine limited ();​
  // executes fine limited (); ​
  // does not execute 
  ```


3. Create a function that will set the color, font­size, and background color of a DOM element. 
  1. If there are fewer arguments, it should place a default value.  
  2. Use the "this" parameter to access the values of the DOM element. (e.g. this.color or this.style.color) 

4. Create a function that can copy either all or specific properties of an object into another. 

 
  ```  
    The functionality should depend on the arguments received.  
    // properties of objB are copied onto objA copyProp​(objA, objB); 
    // only properties p1 and p2 from objB are copied over to objA copyProp​(objA, objB, [​“p1”​, ​“p2”​]);  
  ```

5. Create a function that will: 
  1. return the number of vowels in a string 
  2. return the number of digits in a whole number using logarithm operations. Must be the same function. 
 

6. Create a tree structure and a function that will display all of the elements in that tree. The function should not require any change in case the structure changes. 

a. Example of tree structure: 

                A  
             /  |  \ 
           a    b    c 
           |   / \   | \ 
          aa  ba bb  ca  cb 
                         | 
                         cba  
  ```                       
  \\Print Example
    A
      a
        aa
      b
        ba
        bb
      c
        ca
        cb
          cba
  ```
