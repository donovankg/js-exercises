https://repl.it/Dcxq/0

```javascript

function car(){
	this.baseCost = function (){
		return 25000;
	};
}

function fourWheelDrive(car){
	var number = parseInt(car.baseCost());
	return +number + 1500 +" Is the cost for a jeep with four wheel drive";
}

var jeep = new car();
fourWheelDrive(jeep);


```