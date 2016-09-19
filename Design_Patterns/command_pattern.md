https://repl.it/DcZS/0

```javascript
    function kBBook(){
        this.items = [];
      }
      kBBook.prototype ={
        carListing: function(name){
          var fnName = name;
          if(this[fnName]){
            this[fnName](arguments);
          }
  		},
      addCarToList: function(stuff){
          for(var i=1; i<stuff.length; i++){
          this.items.push(stuff[i]);
          }
          console.log(this.items);
        },
      };
      var kBBook1990= new kBBook();
      kBBook1990.carListing("addCarToList",'dodge 1989','ford 1973','jeep 1987');

```
