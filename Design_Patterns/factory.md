https://repl.it/DcVQ/7
  ```javascript
  
function fn(pickAnimal, color, age){
	function Animal(){
		this.animalType = 'blank';
		this.legs = 4;
		this.eyes = 2;
		this.size = 'med';
		this.speed = "normal";
		this.diet = "beans";
		this.says = "blank";
		this.age = "age";
	}
	var x = new Animal();
	if(pickAnimal =="cat"){
		Cat();
	}else if(pickAnimal == "dog"){
		Dog();
	}
	function Cat(){
		x.animalType = pickAnimal;
		x.diet = "fish";
		x.speed = "slow";
		x.says= 'meow';
		x.age = age;
		x.color = color;
		console.log(x);
	}
	function Dog(){
		x.animalType = pickAnimal;
		x.diet = "bacon";
		x.speed = "fast";
		x.says = "woof";
		x.age = age;
		x.color = color;
		console.log(x);
		}
}
fn('cat', 'yellow','10');
fn('dog', 'brown', '14');
```
