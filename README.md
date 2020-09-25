# **🤫  What-I-learned-in-week-2**<br>
<!-- return, indices, Comparison Operators && if... else (statements), fizzBuzz, codewars-->
> ## **Starting off with reviewing...**<br>
> What are ***JavaScript Functions***?<br>
> A ***JavaScript function*** is a block of code designed to perform a particular task.
> Its executed when ***"something"*** invokes it.<br>

---

## **🤔 what does *return* do ?**<br>
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
Long story short, ***string primitives*** are to my understanding, always parsed, analyzed, solved, looked into the actual string. Where as ***String Objects*** are evaluated as a single string as an object in an **array**.<br>

For example:<br>

```javascript
let example1 = "this is a string";
let example2 = string("this is also a string");
let example3 = new String("this is an object");

console.log(example1);       // "this is a string"
console.log(example2);       // "this is also a string"
console.log(example3);       // [String: "this is an object"]
```

*Now... based on this 👆 we are going to continue with **Indices***

☝️😌 In order to find the type of values we have assigned to those variables we use the `typeof` operator, just like this:

```javascript
typeof example1;        // string
typeof example2;        // string
typeof example3;        // object
```

|  t  |  h  |  i  |  s  |     |  i  |  s  |     |  a  |     |  s  |  t  |  r  |  i  |  n  |  g  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  0  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  |  10 |  11 |  12 |  13 |  14 |  15 |   

We are going to access this 👆 string now and we will be using these following ***operators***:<br>
1. #####  Using only the **square** **brackets** we can access any character in the string
```javascript 
"this is a string"[14]        // n
```
2. ##### 
```javascript 
let example1 = "this is a string";
example1.charAt(8);          // a
```
👆

```javascript 
let example1 = "this is a string";
example1.indexOf("r");       // 12
```
👆

```javascript 
let example1 = "this is a string";
example1.lastIndexOf("s");   // 10
```
👆

```javascript 
let example1 = "this is a string";
example1.indexOf(5);         // is
```
👆

```javascript 
let example1 = "this is a string";
example1.slice(0, 4);        // this
```
👆

```javascript 
let example1 = "this is a string";
example1.slice(10);          // string
```
👆




