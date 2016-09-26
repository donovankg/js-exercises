https://repl.it/Dct8/2

```javascript


    var wrapperFn = (function(){
	var checker;
	function singleton(){
		var speical = "Today's speical is a #2 w/ fries";
		return speical;
	}
	return {
		instnceCheck: function(){
			if(!checker){
				checker = singleton();
				console.log(checker);
			}else{
				return console.log("singleton already ran")
			}
		}
	};
})();

wrapperFn.instnceCheck();
wrapperFn.instnceCheck();


```
