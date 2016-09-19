https://repl.it/Dct8/1

```javascript


    var limitFunc = function(fn, value){
        var count = 0;  
        return function(){
            if(count < value){
            count++;
            fn();
            }
        };
    };
    var limited = limitFunc(function(){
        console.log('this ran');
    },1);
    limited();
    limited();
    limited();


```