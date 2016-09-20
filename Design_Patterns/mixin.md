https://repl.it/DdPo/0
```javascript


  var textBook = function(pageCount, topic){
  	this.pageCount = pageCount;
  	this.topic = topic;
  };
  var histBook = new textBook();
  var values = function (pageCount, topic, Authors){
  	textBook.call(this, pageCount, topic);
  	this.Authors = Authors;
  };
  histBook.prototype = Object.create( textBook);
  var texasHistoy = new values(450,"Texas History",["bob","dan","greg","marry"]);
  console.log( texasHistoy);

```
