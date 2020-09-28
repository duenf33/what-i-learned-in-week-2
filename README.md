# **🤫  What-I-learned-in-week-2**<br>
###### ***Fernando Duenas***
###### ***October 28th, 2020***
<!-- return, indices, Comparison Operators && if... else (statements), fizzBuzz, codewars-->
> ## **Starting off with reviewing...**<br>
> What is a ***JavaScript Function***?<br>
> A ***JavaScript function*** is a block of code designed to perform a particular task.
> Its executed when ***"something"*** invokes it.<br>

---

## **🧐 what does *return* do ?**<br>
The ***return*** statement ends function execution and specifies a value to be returned to the function caller.<br>

For example:
```javascript
function example(num) { 

    return num + 1;
}
console.log(6);     // 7
```
As you can see the *parameter* `num` is assigned the value of number `6` and it `return`s in the function as the sum of `6 + 1` which will equal `7`.<br>

---

> We were also introduce to some new tool of communication such as *Slack*.<br>

## **🤔 What is *Slack* ?**<br>
Slack is a new communication platform to be able to interact with teams, workplaces or friends. It's faster, better organized and more secure than e-mail. It was developed by American software company Slack Technologies. It includes different types of chat rooms that could be created by anyone in the group. It could be organized by topic, private groups and direct messaging.<br>
This is the main platform we will use to communicate in this course.<br>
 
 ---

> This is one of the many important things in javascript. Even though at the moment we are just scratching the surface. This being a very important topic that we need to understand the basis fully in order to advance in this field.<br>

## **🤓 index / indices / ~~indexes~~**<br>
 A string is a sequence of one or more characters that may consist of letters, numbers, or symbols.
 Each character in a JavaScript string can be accessed by an index number, and all strings have methods and properties available to them.<br>
 
 ### 😯 ***The difference between *String Primitives* and *String Object* :***<br>
Long story short, ***string primitives*** are to my understanding, always parsed, analyzed, solved, looked into the actual string. Where as ***String Objects*** are evaluated as a single string, an object in an **array**.<br>

For example:<br>

```javascript
let example1 = "this is a string";

let example2 = string("this is also a string");

let example3 = new String("this is an object");

console.log(example1);       // "this is a string"

console.log(example2);       // "this is also a string"

console.log(example3);       // [String: "this is an object"]
```

---

*Now... based on this 👆 we are going to continue with **Indices***
### ☝️😌 `typeof()`
 In order to find the type of values we have assigned to those variables we use the `typeof` operator, just like this:

```javascript
typeof example1;        // string

typeof example2;        // string

typeof example3;        // object
```
<a id="index"></a>
|  t  |  h  |  i  |  s  |     |  i  |  s  |     |  a  |     |  s  |  t  |  r  |  i  |  n  |  g  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  0  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  |  10 |  11 |  12 |  13 |  14 |  15 |   

We are going to access this 👆 string now and we will be using these following ***operators***:<br>
### **1. Square Brackets**<br> 
Using only the `square brackets` we can ***access any character in the string*** ⇲<br>
```javascript 
"this is a string"[14]        // n
```
### **2. charAt()**<br>
With `charAt(8)` is also possible to return the character just by using the ***index number as parameter*** ⇲<br>
```javascript 
let example1 = "this is a string";

example1.charAt(8);          // a
```
### **3. indexOf()**<br> 
We can use `indexOf("r")` to return the index number by the ***first instance of a character*** ⇲<br>
```javascript 
let example1 = "this is a string";

example1.indexOf("i");       // 2
```
### **4. lastIndexOf()**<br>
`lastIndexOf("s")` is the opposite of `indexOf`. It will get the ***last instance of a character*** ⇲<br>
```javascript 
let example1 = "this is a string";

example1.lastIndexOf("s");   // 10
```
### **5. indexOf()**, *again*<br>
In this `indexOf("is")` method. we can search for multiple characters in the string, where it will return the index number of the first character in the instance ⇲<br>
```javascript 
let example1 = "this is a string";

example1.indexOf("is");       // 5
```
### **6. slice( , )**<br>
The `slice("0, 4")` method returns the characters between these two parameters. The first parameter will include the first character in the return and the second parameter character will not be included, only up to the prior character. In this case ***second parameter number 4*** will be the space between ***this*** and ***is*** ⇲<br>
```javascript 
let example1 = "this is a string";

example1.slice(0, 4);        // this
```
### **7. slice()**<br>
If the ***second parameter*** is not included then the `slice("10")` method will return everything from that parameter to the end of the string ⇲<br>
```javascript 
let example1 = "this is a string";

example1.slice(10);          // string
```
### **8. Length Property**<br>
😏 One more very useful thing is finding the ***length of a string*** and this is how you do it ⇲<br>

```javascript
let thisString = "This is an example";

thisString.length           // 18
```
As you may have noticed, the `length` being `18` is not the same as calling out the `lastIndexOf` of the string. [Remember we have to start counting from `0` to find the index number of a character.](#index) `lastIndexOf` would be `17`.<br>
### **9. toUpperCase()** *and* **toLowerCase()**
😬 Another way of being able to manipulate information input is by changing the letter casing either from lower case to upper case or vice versa because `JavaScript` is case sensitive ⇲<br>
```javascript
let upperCaseInput = "FERNANDO";

upperCaseInput.toLowerCase();       // fernando

let lowerCaseInput = "Duenas";

lowerCaseInput.toUpperCase();       // DUENAS
```
### **Have you notice how the `lowerCaseInput "Duenas"` also have the first character upper cased?**<br>
Well that's the whole point, to be able to transform that input to computer readable without confusion since upper case letters characters are a different `ASCII` code from lower case letters to upper case letters and special characters.

```markdown
* Using ASCII Decimal values:

ASCII value of uppercase A to Z alphabet –> 65 to 90.

ASCII value of lowercase a to z alphabet –> 97 to 122.
```

If you pay attention to the beginning numbers `97` and `65`. If you subtract them `97 - 65`, you will find the result is `32`.<br>
The number `97` is the lower case letter `a` and the upper case `A` would be the number `65` and so on. The distance between `upper case characters` and `lower case characters` in standard ASCII is `32`. 

###### [**click here** to find out more information about this topic in wikipedia.](https://en.wikipedia.org/wiki/ASCII#ASCII_printable_characters)

---

## **🥴 _JavaScript_ Comparison Operators :**<br>

| Name | Shorthand operator | Meaning |
| :--- | :--- | :--- |
| Assignment |	`x = y` |	`x = y` |
| Addition assignment | 	`x += y` |	`x = x + y` |
| Subtraction assignment |	`x -= y` |	`x = x - y` |
| Multiplication assignment |	`x *= y` |	`x = x * y` |
| Division assignment |	`x /= y` |	`x = x / y` |
| Remainder assignment |	`x %= y` |	`x = x % y` |
| Exponentiation assignment |	`x **= y` |	`x = x ** y` |
| Left shift assignment |	`x <<= y` |	`x = x << y` |
| Right shift assignment |	`x >>= y` |	`x = x >> y` |
| Unsigned right shift assignment |	`x >>>= y` |	`x = x >>> y` |
| Bitwise AND assignment |	`x &= y `|	`x = x & y` |
| Bitwise XOR assignment |	`x ^= y `|	`x = x ^ y` |
| Bitwise OR assignment |	`x |= y `|	`x = x | y` |
| Logical AND assignment |	`x &&= y` | `x && (x = y)` |
| Logical OR assignment |	`x ||= y` |	`x || (x = y)` |
| Logical nullish assignment |	`x ??= y` |	`x ?? (x = y)` |
---
The names in this ***table*** are self explanatory, however I am going to explain a couple of them we have not seen yet in class and to be honest it is really interesting to just think of how many different this we can accomplish with the use of these ***operators*** in our code.<br>

We first are going to talk about the shift assignment operators, specially in the example below we will use the `Right Shift Assignment` operator ⇲<br>

```javascript
let num = 90;
num;                      // 90        <- number
result = num.toString(2); // '1011010' <- String
parseInt(result);         // 1011010   <- number
```
* **Right shift assignment ⇲**<br>
```javascript
let num1 = 90;
num1 >>= 1;               // 45
num1.toString(2);         // '0101101'
```
* **Unsigned right shift assignment ⇲**<br>
```javascript
let num2 = 45 >>> 1;
num2;                     // 22
num2.toString(2);         // '0010110'
```
* **Right shift assignment ⇲**<br>
```javascript
let num3 = 22;       
num3 >>= 1;               // 11
num3.toString(2);         // '0001011'
```
* **Right shift assignment ⇲**<br>
```javascript
let num4 = 11 >> 1;
num4;                     // 5
num4.toString(2);         // '0000101'
```
* **Right shift assignment ⇲**<br>
```javascript
let num5 = 5;
num5 >>= 1;               // 2
num5.toString(2);         // '0000010'
```
* **Unsigned right shift assignment ⇲**<br>
```javascript
let num6 = 2 >>> 1;
num6;                     // 1
num6.toString(2);         // '0000001'
```
* **Right shift assignment ⇲**<br>
```javascript
let num7 = 1;
num7 >>= 1;                // 0
num7.toString(2);         // '0000000'
```
---

* ### **`Right/Left Shift Assignment (>>)(<<)` and `Unsigned right/Left shift assignment (>>>)(<<<)`**<br>

As you can see this `Right Shift Assignment` and `Unsigned right shift assignment` operators moves the specified amount of bits to the right and assigns the result to the variable.<br>

Of course there is a lot more than just that. Things always have to get more complicated than what they look like...
<br>

This operator shifts the first operand the specified number of bits to the right. Excess bits shifted off to the right are discarded. Zero bits are shifted in from the left. **The `sign bit` becomes `0`**, so the result is always non-negative.<br>

Yes, now we are talking about `sign bits`... that will be for another topic a different week.

---

* ### **`Logical nullish assignment`**
The nullish coalescing operator (??) is a logical operator that returns its right-hand side operand when its left-hand side operand is null or undefined, and otherwise returns its left-hand side operand.<br>

Contrary to the logical OR (||) operator, the left operand is returned if it is a falsy value which is not null or undefined. In other words, if you use || to provide some default value to another variable foo, you may encounter unexpected behaviors if you consider some falsy values as usable (eg. '' or 0). See below for more examples.<br>

```javascript
const foo = null ?? 'default string';
console.log(foo);     // output: "default string"

const baz = 0 ?? 42;
console.log(baz);     // output: 0
```
In the example below, we will provide default values but keep values other than null or undefined.
```javascript
const nullValue = null;
const emptyText = ""; // falsy
const someNumber = 42;

const valA = nullValue ?? "default for A";
const valB = emptyText ?? "default for B";
const valC = someNumber ?? 0;

console.log(valA); // "default for A"
console.log(valB); // "" (as the empty string is not null or undefined)
console.log(valC); // 42
```
###### [**Click here** for more information about `Logical nullish assignment`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Nullish_coalescing_operator)
---

## **If... Else statement**<br>
The `if statement` executes a statement `if` a specified condition is [truthy](https://developer.mozilla.org/en-US/docs/Glossary/truthy). `If` the condition is [falsy](https://developer.mozilla.org/en-US/docs/Glossary/falsy), another statement can be executed.<br>

For example ⇲<br>
```javascript
function howLongIsMyString(str) {
  let x = str.length;
  if (x > 20) {
    return "That's a long string!";
  } else if (x >= 10) {
    return "That's a regular sized string!";
  } else {
    return "That's a small string!";
  }
}
```

Multiple if...else statements can be nested to create an else if clause. Note that there is no elseif (in one word) keyword in JavaScript.

```javascript
if (condition1)
  statement1
else if (condition2)
  statement2
else if (condition3)
  statement3
...
else
  statementN
```
###### [**Click here** to learn more about If... else... else if... statements](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/if...else)

---

## **FizzBuzz**
FizzBuzz is a classic programming task, usually used in software development interviews to determine if a candidate can code.<br>

Write a function that for multiples of three print “Fizz” instead of the number and for the multiples of five print “Buzz”. For numbers which are multiples of both three and five print “FizzBuzz”.<br>

```javascript
function fizzy(num) {
    if (i % 15 == 0) console.log("FizzBuzz");
    else if (i % 3 == 0) console.log("Fizz");
    else if (i % 5 == 0) console.log("Buzz");
    else console.log(i);
}
```

###### [**Click here to learn more about ⇢**Breaking down the shortest **FizzBuzz** answer and understanding how it works](https://codeburst.io/javascript-breaking-down-the-shortest-possible-fizzbuzz-answer-94a0ad9d128a)