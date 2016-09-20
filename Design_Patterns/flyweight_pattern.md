https://repl.it/DdSu/0

```javascript

  function carLot(carType){
  	carsInLot=[];
  	return{
  		add: function(model, year, milage){
  			carsInLot.push(year+': '+model+' with '+' '+milage);
  		},
  		showList: function(carType){
  			console.log(carsInLot);
  		}
  	};
  }
  
  function carList(carType){
  	var listOfCars= new carLot();
  	listOfCars.add('ford','1980','70,000');
  	listOfCars.add('jeep','1992','50,000');
  	listOfCars.add('jeep','1981','73,000');
  	listOfCars.add('dodge','1984','78,000');
  	listOfCars.add('dodge','1990','100,000');
  	listOfCars.add('jeep','1983','170,000');
  	listOfCars.showList(carType);
  }
  carList();
```
