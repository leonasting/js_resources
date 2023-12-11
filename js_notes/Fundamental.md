
## 1. Variables & function

```
var x = 10; var y = 20;
# Es6
let x = 10; let y = 20;
# function
function add( a, b ) { return a + b; }
let result = add(x, y);
console.log(result);

```

## 2. Conditional statement and Array

```
let a = 20, b = 30; function divide(a, b) { 
if(b == 0) 
{ 
throw 'Division by zero';
} 
return a / b;
}
#array
let items = [1, 2, 3];
# for Loop
for(let i = 0; i < items.length; i++) { console.log(items[i]); }
# for loop 
for(let item of items) { console.log(item); }


```

## 3. Async and defer

- The `async` attribute of the `<script>` element instructs the web browser to fetch the JavaScript file in parallel and then parse and execute it as soon as the JavaScript file is available.
- The `defer` attribute of the `<script>` element allows the web browser to execute the JavaScript file after the document has been parsed.

```
<head> <meta charset="UTF-8">
<title>JavaScript defer demonstration</title> 
<script async src="service.js"></script>
<script async src="app.js"></script>
<script defer src="defer-script.js"></script>
</head>
```

## 4. Comment and block

```
// single line
/**/ - multiline

;  - end of statement
{} - block statement.
```

## 5. Keywords

|[`break`](https://www.javascripttutorial.net/javascript-break/)|`case`|`catch`|
|[`continue`](https://www.javascripttutorial.net/javascript-continue/)|`debugger`|`default`|
|[`else`](https://www.javascripttutorial.net/javascript-if-else/)|`export`|[extends](https://www.javascripttutorial.net/es6/javascript-inheritance/)`||`[import](https://www.javascripttutorial.net/nodejs-tutorial/nodejs-es-module/)`|
|`new`|`return`|`super`|
|`throw`|`try`|`null`|
|`void`|[while](https://www.javascripttutorial.net/javascript-while-loop/)|`with`|
|[`class`](https://www.javascripttutorial.net/es6/javascript-class/)|`delete`|`finally`|
|[in](https://www.javascripttutorial.net/javascript-for-loop/)|[switch](https://www.javascripttutorial.net/javascript-switch-case/)|`typeof`|
|`yield`|[const](https://www.javascripttutorial.net/es6/javascript-const/)|[`do`](https://www.javascripttutorial.net/javascript-do-while/)|
|[for](https://www.javascripttutorial.net/javascript-for-loop/)|instanceof|[this](https://www.javascripttutorial.net/javascript-this/)`|
|`var`|

|`enum`|`implements`|`let`|
|`protected`|`private`|`public`|
|`await`|`interface`|`package`|

|`implements`|`public`|

## 6.Data types
![[JavaScript-data-types.svg]]

**Note:** JavaScript is a dynamically typed language.


Undefined - Not initialized variable.
Null - It is defined/initialized but it not holds null.
number - Real / Floating point integers  (**NaN**)
```
console.log(Number.MAX_VALUE); // 1.7976931348623157e+308 console.log(Number.MIN_VALUE); // 5e-324
console.log('a'/2); // NaN; - Special type of number for holding Not a number
```
String - `'content' or "content"`

boolean -

```
let inProgress = true; 
let completed = false; 
console.log(typeof completed); // boolean
```

Symbol - a function
```
let s1 = Symbol();
console.log(Symbol() == Symbol()); // false
```

BigInt - whole number larger than 2^53 – 1 and notice n at the end.
```
let pageView = 9007199254740991n; console.log(typeof(pageView)); // 'bigint'
```

object type - Collection of properties(key-val)

```
let person = { firstName: 'John', lastName: 'Doe' };
let contact = { firstName: 'John', lastName: 'Doe', email: 'john.doe@example.com', phone: '(408)-555-9999', address: { building: '4000', street: 'North 1st street', city: 'San Jose', state: 'CA', country: 'USA' } }
```

To access a object’s property, you can use

- The dot notation (`.`)
- The array-like notation (`[]`).