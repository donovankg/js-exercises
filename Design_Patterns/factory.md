https://repl.it/DcVQ/12
  ```javascript
  
function AnimalFactory(pickAnimal, color, age){

		this.animalType = pickAnimal;
		this.legs = 4;
		this.eyes = 2;
		this.size = 'med';
		this.speed = "normal";
		this.diet = "beans";
		this.says = "blank";
		this.age = "age";

	this.createAnimal = function(age,color){
		if(this.animalType == "cat"){
			return new Cat(age,color);
		}else if(this.animalType == "dog"){
			return new Dog();
		}else{
			return "error";
		}
	};
	
	function Cat(age,color){
		this.animalType = pickAnimal;
		this.diet = "fish";
		this.speed = "slow";
		this.says= 'meow';
		this.age = age;
		this.color = color;
	}
	function Dog(age, color){
		this.animalType = pickAnimal;
		this.diet = "bacon";
		this.speed = "fast";
		this.says = "woof";
		this.age = age;
		this.color = color;
		}
}
var catFac = new AnimalFactory('cat');
var cat1 =  catFac.createAnimal('10','yellow');
var dogFac = new AnimalFactory('dog');
var dog1 = dogFac.createAnimal("14","brown");
console.log(cat1);
console.log(dog1);
```
