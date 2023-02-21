JAVASCRIPT NOTES

ECMASCRIPT : 
 It is a standard on which java script is based, suppose if you want to add any feature in java script  then you need to add it first in ecmascript.
Ecmascript act as a common place or standard  for adding new features into the javascript
Example from history : Earlier during 1990s when javascript is evolving every developer or contributer is adding new functionalites/features in java script but that is not globally added it was just    added/supported  into their local machines so to reslove this problem ecmascript was used as a common place/standard to add new feature so that every javascript user can use that feature. 

Ways of Executing a javascript :

1. Browser:
      Javascript can be run on any browser by right clicking on the new tab then selecting inspect (or F12 ) then selecting console and in the console you can type and enter to execute
Example: console.log("hello world");

2.  Using Script Tag of Html Document :
      Another way of executing is by inserting javascript code inside the script tag of html document

Example 1:
 <!DOCTYPE html>
<html>

   <head>
      <title>Javascript External Script</title>
      <script src = "/html/script.js" type = "text/javascript"/></script>
   </head>

   <body>
      <input type = "button" onclick = "Hello();" name = "ok" value = "Click Me" />
   </body>

</html>

Example 2:
a) we define a small function using JavaScript in script.js 

function Hello() {
alert("Hello, World");
}

b)  Now use above external JavaScript file in our following HTML document −

 <!DOCTYPE html>

<html>

   <head>
      <title>Event Handlers Example</title>
      <base href = "https://www.tutorialspoint.com/" />
      
      <script type = "text/JavaScript">
         function EventHandler() {
            alert("I'm event handler!!");
         }
      </script>
   </head>

   <body>
      <p onmouseover = "EventHandler();">Bring your mouse here to see an alert</p>
   </body>

</html>

3. Runtime Execution using Node.js
   Install node.js and run javascript in it

4. Using Online Website interpreters 

Example: replit 
 https://replit.com

Syntax Meaning / Defination : 

Just like we follow rules while speaking english (the grammer), we have some rules to follow while writing a javascript program. the set of these rules is called syntax in javascript.

Variables in Javascript

Variable is the name of the memory location used to store the value
The value of a javascript varaible can be changed during the execution of a program 
Variable can be used using the let, var or const keyword but using var keyword for a variable may results in bugs in some conditions so it is better to use the let keyword for varaibles.

Variable Syntax :
let variable name =  value ;
  or
var variable name  = value;

Variable Example :
let name = wajeed;
let a = 10;
var a = 10;

Rules for  naming  a variable
 Only letters, digits, underscore ( _  ) ,, and $ sign is allowed in a  javascript varaible name
 Varaible name must begin with a letter, $ or underscore
 Javascript reserved words cannot be used as a variable name
 Wajeed and wajeed are different varable name (i.e Javascript is  Case sensitive)

Types of variable identifiers

 var vs let vs const

1. var is globally socped while let and const are locally scoped
Ex : 
        var a = wajeed;
        let  b = md;
        {
        var a = wajs;
        let b = mmdd
        console.log(a)
        console.log(b)
        }
        console.log(a)
        console.log(b)
Output: 
   wajs
   mmdd
   wajs
   md
As var is a globally scoped variable so if you re-declare the var in the blcok then the re-declared value or updated value of varaible will be printed and the first declared value will be discarded but if you re declare the let variable in a block then that re declared value will be printed within that block and outside the block the original value or the first declared value will be printed as showed in above example

2. Var vaiable can be updated and re declared within its scope or bolck but let and const cant be re declared within the smae block or within the same scope but let can be updated and const cannot be updated.
Ex: 
     var a = wajeed  // Declaring 
     var a = waj        // re declare
     a =  wajjs          // updating 
     
     let b = javascript   // Declaring 
     let b = java          // throws error as redeclaring is not allowed in let varaibles
          b = jav            //  updating is allowed in let 
3.  Const can niether be updated nor be  re-declared
4.  Var variable can be initilized with the undefined but let and const cannot be initilized with undefined 
   Ex:    
            Var a = undefined;
            let b = undefined; // throws error as not allowed in let and const.
5. Const must be initilized unlike let and char
   Ex:    
            Var a;      // allowed in var
            Let b;      // allowed in let
            Const a;  // throws error as const must be initilized

Data types in Java script

 Primitive Data types :  
 The predefined data types provided by JavaScript language are known as primitive data types. Primitive data types are also known as in-built data types.
    Primitive data types are a set of basic datat types in javascript.
     In JavaScript, a primitive (primitive value, primitive data type) is data that is not an object and has no methods or properties. 
     There are following 7 primitive data types: 
         
1. Null  
     let a = null;
2. Number
      let b = 20;
3. String
      let c = "wajeed";
4. Symbol
      let d = Symbol("I am a symbol of excellence")
5. Bigint
      let e = Bigint("700") + Bigint("77")
     o/p e = 777
6. Boolean
      let wajeed = true;
7. Undefined
       let f = undefined or let f;
Non Primitive Data types :  
  The data types that are derived from primitive data types of the JavaScript language are known as non-primitive data types. It is also known as derived data types or reference data types.
 1. Object :    
  Object is a non primitive data type in javascript
  Object in Javascript is an entity having properties and methods.

Creation of objects:

  1. Using Constructor Function to define an object:
// Create an empty generic object
var obj = new Object();
Ex:
// Create a user defined object
var mycar = new Car();
   2. Using Literal notations to define an object:
// An empty object
var square = {};
Ex:
// Here a and b are keys and
// 20 and 30 are values
var circle = {a: 20, b: 30};

2.Array