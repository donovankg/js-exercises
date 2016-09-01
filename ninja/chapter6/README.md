  1. Create a set of object types that describe a series of related objects that may share behavior and/or attributes. Code the example and another set of classes different from                         the example. Add properties/methods as needed.  

    Example: 
    
    ```javascript
    Shape //{ pEdges, fnDisplay } 
    Quadrilateral is Shape //{ fnArea, fnPerimeter}  
    Square is Quadrilateral //{ } 
    Triangle is Shape //{fnArea, fnPerimeter} 
    ```
    Use of inheritance, prototype, and function overwriting. 
    ```javascript
    function Shape(color){
	this.pEdges= 0;
	this.fnDisplay = true;
	this.color = color;
}
//children
function Quadrilateral(color){
	fnArea = 'This is the area';
	fnPerimeter = 'This is the perimeter';
	Shape.call(this, color);
}
function Triangle(color){
	this.size = 'small';
	this.color = color;
	Shape.call(this, color);{
	this.pEdges = 3;
	}
}
//grandchild
function Square(color){
	this.size= "med";
	this.color = color;
	Quadrilateral.call(this, color);
	this.pEdges = 4;
}


Quadrilateral.prototype = new Shape();
Square.prototype = new Quadrilateral();

Shape.prototype.test=function(){
	return " These are both shapes.";
};
var sqr = new Square('red');
var tri = new Triangle('orange');
console.log(sqr);
console.log(tri);
console.log(sqr.test());
```
