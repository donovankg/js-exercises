1. Given the following HTML markup, create a JS function that can print out the attributes                             of the DOM elements: 

https://repl.it/Dc0g/4
```javascript
        //Example: 
        printAttr (el, [‘id’, ‘class’, ‘style’, ‘val’]); 
        // should print out: 
        // a 
        // square 
        // display:inline­block // something important 
        var el = document.getElementById("a");
        function printAttr(elem, arr){
        	for(var i = 0; i < arr.length; i++){
        		//console.log(arr[i]+" = "+el.getAttribute(arr[i]));
        		console.log(el.getAttribute(arr[i]));
        	}
        }
        
        printAttr (el, ['id', 'class', 'style', 'val']);
        printAttr (el, ['id', 'val']);
        printAttr (el, ['stuff', 'stuff2']);

```
Use of built in JS functionality for attribute retrieval 

