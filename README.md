# Javascript-Basics
Lets learn basics of Javascript 
<br><br><br>
<h2>Declaration of a Variable</h2>
<br><br><br>
<img src="js basics.png">
<br><br><br>
console.log(`Here Veeru's age is ${$VeeruAge} and Jay's Age is ${$JayAge}`);<br>


```javascript

// Truthy and false values<br>
// Their are 5 values which gives a false boolean value<br>
// This are: "", 0 , null, NaN, Undefined<br>
// To convert a values to boolean using boolean();<br>
console.log(Boolean(0));<br>
console.log(Boolean("")); // Here "" Empty string is a False<br>
console.log(Boolean('Jonas')); // string are true<br>
console.log(Boolean({})); // An empty object is a true value<br>
<br>
let $null = Number("Hello"); // Here we are converting string to number but here we are trying to<br>
//convert character so it shows NaN as output so "NaN" is False<br>
console.log($null); // False<br>
<br>
// The conversion is not done Explicitly but implicitly using cocersion<br>
// it can be done by two ways using logical operators and another if else statement<br>
<br>
let balance = 0;<br>
if(balance){ // here because if else statement get executed when the values are true<br>
  console.log("Don't Spend on Usless Stuff"); // it won't get displayed<br>
}else{<br>
    console.log(`Go to work bro`); // This Will be Displayed<br>
}<br>
<br>
// lets test with Undefined<br>
let $undef; // if you get a value to the varible then it will display the first one<br>
if($undef){<br>
   console.log(`Value defined`);<br>
}<br>
else{<br>
    console.log(`Value not Defined`);<br>
}
```


```js
// Equality Operators === & ==<br>
// Here loose equality : == is does not check the value lossly means it don't care what type it is<br>
// if the value matches the it is true<br>
// But that's not the same with strict equality :=== it checks the values very strictly and its types<br>
// Here we will find out the age of ali and find out weather he is adult of not<br>
// Or the value is true or False<br>
<br>
let Ali = 18; // 18 is in a number form<br>
if(Ali === 18) console.log("ALi is an Adult"); // it will definitely show up true and displayes 1st statement<br>
else console.log(`YOu are not a adult`); // but what if the input in type string<br>
<br>
if(18 == "18") console.log("!Yup converted"); // == converts string to number<br>
<br>
if(18 === "18"){ // Because === It does not converts cocersion<br>
    console.log("NOt Converted");<br>
} else{ console.log("Strict operator doesn't do coersion");<br>
}<br>
// here strict operator === does not perform type cocersion but == loose one does<br>
<br>
// both works the some<br>
// But if we change the 18 to string then the loose one be displayed<br>
Ali = "18";<br>
if(Ali === 18) console.log(`ALi is adult (Strict ===)`);<br>
if (Ali == 18) console.log(`Ali is adult (loose ==)`);                                    //no need of flower bracket if we are using oneline<br>
// Here both get displayed because 18 = 18 as the main common thing in both of these is they<br>
// only becomes true when both the sides matches<br>
// == Equality is good but brings all of bugs with it<br>
// So avoid as much as you can to get clean code and use the ===<br>// try to use === to compare the values most of the pro developers use it<br>// rather than depending of type cocersion convert the values manually<br>// by using toNumber() function use === as default<br>// Pretend that == does even exists<br>// Here a Example for how to convert the string to number and use ===<br><br>// Prompt is a attribute to take input from user on webpages<br><br>
prompt(`Enter Your Age`);<br>
// Only prompt doesn't Store or display value in the console to save or work<br>
// with those value declare it in a varibles<br>
// here prompt gives out string even if you enter any value is will be taken in as string<br>
<br>
// Here we have a donut Shop and This shop sell standard packs of donuts<br>
// Different packs contains different number of donots which are with pack of 5, 7, 9, 10<br>
// try to sugest people for pack of 10<br>
<br>
<br>
```

```javascript
/* Here as said that prompt understand any value enter as string but we want a<br>
number as input because we are not gonna use loose(==) so to manually convert<br>
the string use Number() */<br>
let CustomerChoice = (Number(prompt(`What Pack of Donuts Will you like to have \n We have Pack of 5, 7, 9, 10 ` )));<br>
let RecommendedPack = 10; // we are recommending pack of 10<br>
<br>
// First lets compare the customers choice with pack of 10<br>
if(CustomerChoice === 10){<br>
    // If 10 this will be displayed<br>
    console.log("Thanks for buying Our most Sold Pack (10)")<br>
} else if(CustomerChoice === 9){<br>
    // If 9 this will be displayed<br>
    console.log("Thanks for Buying the Second most loved pack (9)");<br>
} else if(CustomerChoice === 7){<br>
    // If 7 this will be displayed<br>
    console.log("Thanks for Buying the Budget Friendly pack (7)");<br>
} else if(CustomerChoice === 5){<br>
    // If 5 this will be displayed<br>
    console.log("Thanks for buying the Mini pack (5)");<br>
} else{<br>
    // If consumer enters any different values other than mention above this one will be displayed<br>
    console.log("We don't Sell Loose donuts");<br>
+}<br>
+<br>
// It only gets displayed when you enter value other than 10<br>
<br>
// Here this condition is trying to say that if the customers choice does not match<br>
// to the recommended pack this statement will be displayed<br>
// Test it on website<br>
if(CustomerChoice !== RecommendedPack){<br>
    console.log("Try to buy pack of 10 next time");<br>
}<br>
<br>
```
