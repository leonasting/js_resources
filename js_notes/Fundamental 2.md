## 1.  Numeric Separator
- Use underscores (`_`) as the numeric separators to create a visual separation between groups of digits.
```
// BigInt 
const max = 9_223_372_036_854_775_807n;
// binary 
let nibbles = 0b1011_0101_0101; 
// octal 
let val = 0o1234_5670; 
// hex 
let message = 0xD0_E0_F0;
```
[[example]]

Example
```
## 2 .Octal and binary


- Octal literals start with `0o` followed by a sequence of numbers between 0 and 7.
- Binary literals start with `0b` followed by a sequence of numbers 0 and 1.
```
let f = 0b111; console.log(f); // 7
let c = 0o51; console.log(c); // 41
```

## 3. Boolean object vs boolean primitive
First, `active` is an object so you can add a property to it:

```
let completed = true; 
let active = new Boolean(false);
active.primitiveValue = active.valueOf();
console.log(active.primitiveValue); // false
console.log(typeof completed); // boolean 
console.log(typeof active); // object
console.log(completed instanceof Boolean); // false
console.log(active instanceof Boolean); // true

```

## 4. Arithmetic operators

+,-,\*,/,  - Basic operators
% - modulo/remainter

## 5. Handling Binary and Octal

n ES5, JavaScript didn’t provide any literal form for binary numbers. To parse a binary string, you use the `parseInt()` function as follows:

`let e = parseInt('111',2); console.log(e); // 7`

ES6 added support for binary literals by using the `0b` prefix followed by a sequence of binary numbers (0 and 1). Here is an example:

`let f = 0b111; console.log(f); // 7`

## 6. Unary Operators

|Unary Operators|Name|Meaning|
|---|---|---|
|+x|Unary Plus|Convert a value into a number|
|-x|Unary Minus|Convert a value into a number and negate it|
|++x|Increment Operator (Prefix)|Add one to the value|
|–x|Decrement Operator (Prefix)|Subtract one from the value|
|x++|Increment Operator (Postfix)|Add one to the value|
|x–|Decrement Operator (Postfix)|Subtract one from the value|


## 7. comparison

|Operator|Meaning|
|---|---|
|<|less than|
|>|greater than|
|<=|less than or equal to|
|>=|greater than or equal to|
|\==|equal to|
| \!= | not equal to|
|\===| strict equal with type|
|\!==| not strict equal with type|

