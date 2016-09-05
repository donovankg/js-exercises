1. Create a function that will transform a hex number into an rgb format. 

        Example: 
        
        function hex2rgb(value){
                var hex = parseInt(value.substring(1), 16);
                var r = (hex & 0xff0000) >> 16;
                var g = (hex & 0x00ff00) >> 8;
                var b = hex & 0x0000ff;
                return [r, g, b];
        }

        console.log(hex2rgb('#3020ff'))
        //output
        “#3020ff”  →  “rgb ( 48, 32, 255)”


  Use of regular expressions 
  
2. Create a function that will transform a U.S style date format into a format of a different                                 language/region. If that date is a holidays on the target locale (language & region), it                             should be mentioned. ​Preferably, use a different language from that of the example. 

        Example: 
        English­US: 09/16/2014 → Spanish­MX: 16/09/2014 (Dia de la independencia)  
        Spanish­MX: 1/4/2014 → English­US: 4/1/2014 (April fools day) 
        
  Use of regular expressions, and lookup tables 
  
3. Write an expression that would satisfy at least one match for: 
  1. .abc       something else.abc
  2. a+b?!!1{4}         ab!!1111
  3. .{3}a\.b   123a1b
  4. \w 'hi'    (word character)
  5. \s ' '     (whitespace)
  6. \d 2       (digit)
  7. . 
  8. [abc]      a
  9. (abc)      abc
  10. [a­zA­Z_\$\.]+[A­Za­z_\$0­9\.]*@[a­zA­Z_\$\.]+[a­zA­Z_\$0­9\.]*\.(com|net|org){1}         donovan1@email.net 
  11. \([0oOn]{1}(_|\s)[0oOn]{1}\)      o|o

4.  Write a regular expression that can match: 

  1. Date format <Month­string> <##day>, <####year> 
        
          Examples:
          1. September 29, 1972 
          2. February 99, 0001 
          3. June 04, 3000 
      
                <####day>./(\d+),\s?(\d+)/
  2. A letter followed OR preceded by a number 
    
          Examples:
          1. A52 
          2. d747 
          3. 27X 
          4. v2 
                /\d*([a-zA-Z])\d*/g
  3. txt, java, and cpp files with names consisting of only letters 
    
          Examples: 
          1. test.java 
          2. program.cpp 
          3. newReport.txt 
                /\.(\w{3})/
  4. A 5 character palindrome 
  
          Example:
          1. abcba 
          2. 12321 
          3. _1a1_ 
                /(.)(.).\2\1/
  5. All words that consist of letters from b to y only 
         
          Example 
          input​: “Bee zapp Crow Eagle Zorro  mouse Ape  you” 
          output​: [“Bee”,”Crow”,”mouse”,”you”]
                /*[b-y]*/

  6. All the non nested tag elements in a string 

          Example 
          input​: “Is <b>4 < ­1/12</b> true? The <b>answer</b> will <em>surprise</em> you.” 
          output​: <b> 4 < ­1/12</b>, <b>answer</b>, <em>surprise</em> 
                /<(\w*)>(.*?)<\/\1>/g

5. Write a program that will: 

  1. Shift cyclically every letter of the alphabet by one, and the numbers as well. 
    
          Example
          1. aBc = bCd 
          2. xyz = yza 
          3. aK89 = bL90 

  2. From a reasonably sized text, have a user defined string be replaced by that same string with a hashtag.
  That hashtag should be a link for a twitter search as well.  

          Example
          text: ...should never use yolo for any reason...
          input. String: yolo 
          output. ... should never use #yolo for any reason ...  
