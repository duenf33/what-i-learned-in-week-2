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

*Now... based on this 👆 we are going to continue with **Indices***

☝️😌 In order to find the type of values we have assigned to those variables we use the `typeof` operator, just like this:

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
##### 1. Using only the `square brackets` we can ***access any character in the string*** ⇲<br>
```javascript 
"this is a string"[14]        // n
```
##### 2. With `charArt(8)` is also possible to return the character just by using the ***index number as parameter*** ⇲<br>
```javascript 
let example1 = "this is a string";

example1.charAt(8);          // a
```
##### 3. We can use `indexOf("r")` to return the index number by the ***first instance of a character*** ⇲<br>
```javascript 
let example1 = "this is a string";

example1.indexOf("i");       // 2
```
##### 4. `lastIndexOf("s")` is the opposite of `indexOf`. It will get the ***last instance of a character*** ⇲<br>
```javascript 
let example1 = "this is a string";

example1.lastIndexOf("s");   // 10
```
##### 5. In this `indexOf("is")` method. we can search for multiple characters in the string, where it will return the index number of the first character in the instance ⇲<br>
```javascript 
let example1 = "this is a string";

example1.indexOf("is");       // 5
```
##### 6. The `slice("0, 4")` method returns the characters between these two parameters. The first parameter will include the first character in the return and the second parameter character will not be included, only up to the prior character. In this case ***second parameter number 4*** will be the space between ***this*** and ***is*** ⇲<br>
```javascript 
let example1 = "this is a string";

example1.slice(0, 4);        // this
```
##### 7. If the ***second parameter*** is not included then the `slice("10")` method will return everything from that parameter to the end of the string ⇲<br>
```javascript 
let example1 = "this is a string";

example1.slice(10);          // string
```

---

😏 One more very useful thing is finding the ***length of a string*** and this is how you do it :<br>

```javascript
let thisString = "This is an example";

thisString.length           // 18
```
As you may have noticed, the `length` being `18` is not the same as calling out the `lastIndexOf` of the string. [Remember we have to start counting from `0` to find the index number of a character.](#index) `lastIndexOf` would be `17`.<br>

---

😬 Another way of being able to manipulate information input is by changing the letter casing either from lower case to upper case or vice versa because `JavaScript` is case sensitive.<br>
```javascript
let upperCaseInput = "FERNANDO";

upperCaseInput.toLowerCase();       // fernando

let lowerCaseInput = "Duenas";

lowerCaseInput.toUpperCase();       // DUENAS
```
**Have you notice how the `lowerCaseInput "Duenas"` also have the first character upper cased?**<br>
Well that's the whole point, to be able to transform that input to computer readable without confusion since upper case letters characters are a different `ASCII` code from lower case letters to upper case letters and special characters.

```markdown
* Using ASCII Decimal values:

ASCII value of uppercase A to Z alphabet –> 65 to 90.

ASCII value of lowercase a to z alphabet –> 97 to 122.
```

If you pay attention to the beginning numbers `97` and `65`. If you subtract them `97 - 65`, you will find the result is `32`.<br>
The number `97` is the lower case letter `a` and the upper case `A` would be the number `65` and so on. The distance between `upper case characters` and `lower case characters` in standard ASCII is `32`. 

###### [click here to find out more information about this topic](https://en.wikipedia.org/wiki/ASCII#ASCII_printable_characters)

---

## **🥴 _JavaScript_ Comparison Operators && if... else (statements) :**<br>





