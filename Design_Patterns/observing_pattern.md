https://repl.it/DcLi/0

```javascript

    function ObserverList() {
        this.observerList = [];
    }
    ObserverList.prototype.add = function(observer) {
        this.observerList.push(observer);
    }
    ObserverList.prototype.remove = function(observer){
    	this.observerList.splice(this.indexOf(observer),1);
    };
    ObserverList.prototype.count = function() {
        return this.observerList.length;
    };
    ObserverList.prototype.indexOf = function(observer) {
         for (var i = 0; i < this.observerList.length; i++) {
            if (this.observerList[i] === observer) {
                return i;
            }
        }
    };
    ObserverList.prototype.getObserver = function(index) {
        return this.observerList[index];
    };
    /*Subject*/
    function Subject() {
        this.observers = new ObserverList();
    }
    Subject.prototype.addObserver = function(obj) {
        this.observers.add(obj);
    };
    Subject.prototype.removeObserver = function(obj) {
        this.observers.remove(obj);
    };
    Subject.prototype.notify = function(value) {
        var i;
        for (i = 0; i < this.observers.count(); i++) {
            this.observers.getObserver(i).update(value);
        }
    };
    function Observer(){
    	this.update = function(){
    		/*best implemented in the concrete type*/
    	};
    }
    var extend = function(obj, interface){
    	
    	for(var key in interface){
    		obj[key] = interface[key];
    	}
    }
    window.onload = function() {
    	extend(subject, new Subject());
    	extend(observer1,new Observer());
    	extend(observer2,new Observer());
    	extend(observer3,new Observer());
    	subject.addObserver(observer1);
    	subject.addObserver(observer2);
    	subject.addObserver(observer3);
    	subject.addEventListener('keyup',function(){
    		this.notify(this.value);
    	},false);
    	observer1.update = function(val){
    		this.innerHTML = val;
    	}
    	observer2.update = function(val){
    		this.innerHTML = val;
    	}
    	observer3.update = function(val){
    		this.innerHTML = val;
    	}
    };

```
