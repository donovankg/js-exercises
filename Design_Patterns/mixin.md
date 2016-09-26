https://repl.it/DdPo/2
```javascript


 var Books = function(histType, Author){
	this.textBook = function(){
		return "you have selected: "+subjectHist()+getAuthor();
	};
	var subjectHist = function(){
		if(histType = "texas"){
			return "Texas History, ";
		}else{
			return "unknown histoy type, ";
		}
	};
	var getAuthor = function(){
		if(Author = 'jim'){
			return 'Jim Smith';
		}else{
			return 'unknown author';
		}
	};
};
var histBook = new Books();
histBook.textBook('texas','jim');

```
