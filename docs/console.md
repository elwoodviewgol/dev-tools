# Console

## Basic Console  
   
### Execute JavaScript  
Run JavaScript in the directly in the console.
```js 
alert("I Am An Alert");  // Execute JavaScript to fire an alert message.  
  
1 // Returns '1'  
  
1+3 // Returns '4'  

```  
  
---  
  
### '$_' Money Sign + Underscore
```js 
$_ // Gives the last returned value.   
  
$_0 // Last element inspected by the selector.  

$_1 // The element before the last last element inspected by the selector.  
  
$_2 // So on and so forth.  

``` 

### '$' Alias
  
Use the '$' as an alias for [Document.querySelector()](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)
```js  
document.querySelector('h1').style.color = 'red'; // Vanila JavaScript  
  
$('h1').style.color('aqua');
```  
---  
  
### Console.  
  
Log different things to the console  
```js
// .CLEAR  
console.clear();

// .LOG - Plain Text
console.log("I Am A Logged Value...");  

// .LOG - Variable
console.log("I Am A Logged Value...");  

// .ERROR
console.error("I Am A Logged Error...");  

// .WARN
console.warn("I Am A Logged Warning...");  

// .DIR
console.dir(document);  

// .LOG
console.log(document.URL);  

// .TABLE
console.table([{name: 'John', email: 'john.doe@gmail.com', age:33}]);  
```  
  
#### Groups  
Log groups of values in the console.  
```js  

// GROUPS
console.group('Returned Values');
    console.log('CNN');
    console.log('Local');
    console.log('FOX');
console.groupEnd('Returned Values');
```  
  
#### Time  
Log the time taken to log through a ForLoop  
```js  

// Understanding Time.
console.time('For Loop');
    for( var i = 0; i < 200; i++ ){
        console.log("Looped Value: ", i);
    };
console.timeEnd('For Loop');
```  
   
#### ASSERTION  
Create functions to compare values.  
```js  
function greaterThan(x, y){
    console.assert( 
        x > y, 
        { 
            "message": "X is NOT greater than Y", 
            "X": x, 
            "Y": y
        });
}

greaterThan(1, 5);
```  
