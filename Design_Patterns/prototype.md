https://repl.it/DcTy/2
```javascript
  const toy ={
  	init: function(type){
  		this.type = type;
  	},
  	play: function(){
  		console.log('this toy is a ' + this.type);
  	}
  };
  const car = Object.create(toy);
  car.init('car');
  car.play();
  
  console.log(toy.isPrototypeOf(car));

```
