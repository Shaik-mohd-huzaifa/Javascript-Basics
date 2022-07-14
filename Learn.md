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
// Their are 5 values which gives a false boolean value
// This are: "", 0 , null, NaN, Undefined
// To convert a values to boolean using boolean();
console.log(Boolean(0));
console.log(Boolean("")); // Here "" Empty string is a False
console.log(Boolean('Jonas')); // string are true
console.log(Boolean({})); // An empty object is a true value

let $null = Number("Hello"); // Here we are converting string to number but here we are trying to
//convert character so it shows NaN as output so "NaN" is False
console.log($null); // False

// The conversion is not done Explicitly but implicitly using cocersion
// it can be done by two ways using logical operators and another if else statement

let balance = 0;
if(balance){ // here because if else statement get executed when the values are true
  console.log("Don't Spend on Usless Stuff"); // it won't get displayed
}else{
    console.log(`Go to work bro`); // This Will be Displayed
}

// lets test with Undefined
let $undef; // if you get a value to the varible then it will display the first one
if($undef){
   console.log(`Value defined`);
}
else{
    console.log(`Value not Defined`);
}
```

```js
// Equality Operators === & ==
// Here loose equality : == is does not check the value lossly means it don't care what type it is
// if the value matches the it is true
// But that's not the same with strict equality :=== it checks the values very strictly and its types
// Here we will find out the age of ali and find out weather he is adult of not
// Or the value is true or False

let Ali = 18; // 18 is in a number form
if(Ali === 18) console.log("ALi is an Adult"); // it will definitely show up true and displayes 1st statement
else console.log(`YOu are not a adult`); // but what if the input in type string

if(18 == "18") console.log("!Yup converted"); // == converts string to number

if(18 === "18"){ // Because === It does not converts cocersion
    console.log("NOt Converted");
} else{ console.log("Strict operator doesn't do coersion");
}
// here strict operator === does not perform type cocersion but == loose one does

// both works the some
// But if we change the 18 to string then the loose one be displayed
Ali = "18";
if(Ali === 18) console.log(`ALi is adult (Strict ===)`);
if (Ali == 18) console.log(`Ali is adult (loose ==)`);                                    //no need of flower bracket if we are using oneline<br>
// Here both get displayed because 18 = 18 as the main common thing in both of these is they
// only becomes true when both the sides matches
// == Equality is good but brings all of bugs with it
// So avoid as much as you can to get clean code and use the ===<br>// try to use === to compare the values most of the pro developers use it<br>// rather than depending of type cocersion convert the values manually<br>// by using toNumber() function use === as default // Pretend that == does even exists<br>// Here a Example for how to convert the string to number and use ===<br><br>// Prompt is a attribute to take input from user on webpages
prompt(`Enter Your Age`);
// Only prompt doesn't Store or display value in the console to save or work
// with those value declare it in a varibles
// here prompt gives out string even if you enter any value is will be taken in as string

// Here we have a donut Shop and This shop sell standard packs of donuts
// Different packs contains different number of donots which are with pack of 5, 7, 9, 10
// try to sugest people for pack of 10


```

```javascript
/* Here as said that prompt understand any value enter as string but we want a
number as input because we are not gonna use loose(==) so to manually convert
the string use Number() */
let CustomerChoice = (Number(prompt(`What Pack of Donuts Will you like to have \n We have Pack of 5, 7, 9, 10 ` )));
let RecommendedPack = 10; // we are recommending pack of 10

// First lets compare the customers choice with pack of 10
if(CustomerChoice === 10){
    // If 10 this will be displayed
    console.log("Thanks for buying Our most Sold Pack (10)")
} else if(CustomerChoice === 9){
    // If 9 this will be displayed
    console.log("Thanks for Buying the Second most loved pack (9)");
} else if(CustomerChoice === 7){
    // If 7 this will be displayed
    console.log("Thanks for Buying the Budget Friendly pack (7)");
} else if(CustomerChoice === 5){
    // If 5 this will be displayed
    console.log("Thanks for buying the Mini pack (5)");
} else{
    // If consumer enters any different values other than mention above this one will be displayed
    console.log("We don't Sell Loose donuts");
}

// It only gets displayed when you enter value other than 10

// Here this condition is trying to say that if the customers choice does not match
// to the recommended pack this statement will be displayed
// Test it on website
if(CustomerChoice !== RecommendedPack){
    console.log("Try to buy pack of 10 next time");
}

```
