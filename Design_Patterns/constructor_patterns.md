*Constructor Pattern

Constructor Patterns are used to create specific objects and creating properties / set values into them. 


```javascript
    //The Constructor Pattern example 
    var obj = {};

    //set properties
    //get properties

    //dot syntax
    obj.tires = 4;
    var getTires = obj.tires;
    //square bracket syntax
    var x = 'doors';
    obj[x] = 5;

    var getDoors = obj[x];

    //Object.defineProperty

    Object.defineProperty(obj, "color",{
        value: "red",
        writable: true,
        enumerable: true,
        configurable: true
    });

    //Object.defineProperties
    Object.defineProperties(obj, {
        "radio":{
            value: "works",
            writable: true,
            enumerable: true,

        },
        "headlights":{
            value: "two lights",
            writable:true,
            enumerable: true,

        }
    });
    

    obj.tires = 4;


    console.log(obj);
```