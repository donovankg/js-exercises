1. Create a function that will display a random sentence to the console every minute. 
  
  Basic use of timers 
  ```javascript
      var sentences = {
    	1: 'Lorem Ipsum is simply dummy text of the printing and typesetting industry',
    	2: 'Lorem Ipsum has been the industry`s standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.',
    	3: 'It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.',
    	4: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using `Content here, content here`, making it look like readable English.'
    };
    min = Math.ceil(5);
    max = Math.floor(1);
    test = 0;
    //while (test != 4){
    	function minMax(){	
    		test  = Math.floor(Math.random() * (max-min))+min;
    	}
    var output = setInterval(minMax, 60000);
    console.log(output);
  ```

2. Create functions A, B, and C that execute every 30s, 1min, and 1min 15s respectively.                             Use only 1 timer/interval to control all three functions.  

  use of a central timer controller 

