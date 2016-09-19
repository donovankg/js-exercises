1. Given the following HTML markup, create a JS function that can print out the attributes                             of the DOM elements: 

https://repl.it/Dc0g/0
```javascript
        //Example: 
        printAttr (el, [‘id’, ‘class’, ‘style’, ‘val’]); 
        // should print out: 
        // a 
        // square 
        // display:inline­block // something important 
          function printAttr(elem,ar){
            var attrib =elem.attributes;
            for (var i=0; i<arr.length; i++){
              var k = arr[i];
              console.log(attrib[k].name+":"+attrib[k].value);
              }
          }
          window.onload = function(){
          var el = document.getElementsByTagName('div')[0];
          printAttr(el,['id', 'class', 'when']);
          };
        function assert(value, desc) {
              var resultsList = document.getElementById("results");
              if (!resultsList) {
                resultsList = document.createElement('div');
                document.getElementsByTagName('body')[0].appendChild(resultsList);
                resultsList.setAttribute('id','results');
              }
              var li = document.createElement("li");
              li.className = value ? "pass" : "fail";
              li.appendChild(document.createTextNode(desc));
              resultsList.appendChild(li);
            }
        window.onload = function(){
                    var div = document.getElementsByTagName('div')[0];
                    assert(true,div.getAttribute('id'));
                    assert(true,div.getAttribute('class'));
                    assert(true,div.getAttribute('style'));
                    assert(true,div.getAttribute('val'));
        };    

```
Use of built in JS functionality for attribute retrieval 

