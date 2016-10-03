https://repl.it/DdPo/3
```javascript


var Book = function( author, subject){
	this.ed = "5th edition";
	this.author = author;
};

var PrintCopy = function(author, bookinfo, pubInfo){
	Book.call(this,author);

	this.pubInfo = pubInfo;
	this.bookinfo = bookinfo;
};

PrintCopy.prototype = Object.create(Book.prototype);
var tx6thEd = new PrintCopy ("Greg Allen", ["Tx History",'pages 450'], ["Ny new paper","1234 main street, YNC"]);
console.log(tx6thEd);

```
