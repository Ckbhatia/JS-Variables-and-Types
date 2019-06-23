## If Statement
1.  🎖Make a simple calculator with these functions. Using prompt, type conversion, if else statement. Use prompt to take the input from user i.e two numbers and an operation (Add, Sub, Mul, Div).

  ⛑ Rule
    * [ ] While substracting and dividing keep in mind the number one should be greater then number two. If not show alert saying `Number Two is larger then Number one`.
  ⚡️ Operations
    * [ ] Add
    * [ ] Sub
    * [ ] Mul
    * [ ] Div
```js
let inputFirst = prompt('Enter a number');
let inputTwo = prompt('Enter an another number');
let numFirst = Number(inputFirst);
let numTwo = Number(inputTwo);
let result;
  if ( numFirst > numTwo) {
      let inputThird = prompt("Write operation type's short word that you want,EX: Add, Sub, Mul Or Div");
      if (inputThird === 'Add') {
          result = numFirst + numTwo;
      }
      else if (inputThird === 'Sub') {
          result = numFirst - numTwo;
      }
      else if (inputThird === 'Mul') {
          result = numFirst * numTwo;
      }
      else if (inputThird === 'Div') {
          result = numFirst / numTwo;
      }
      else {
          alert('Please check operation type again');
      }
    }
  else {
	  alert('Number Two is larger than Number one');	
  }
console.log(result);
```


2. 🎖Write a if else statement which checks if the status is single `console.log` the message `John is single` or else `John is married`
```js
var firstName = 'John';
var status = 'single';
// Your code goes here
if(status == 'single') {
  console.log(`${firstName} is ${status}`);
}
else {
  console.log(`${firstName} is married`);
}
```

3. 🎖Write a JavaScript program that takes two `integers` from user (using prompt) and alerts the larger number.
```js
let userInput1 = prompt("Enter a interger");
let userInput2 = prompt("Enter an another interger");

if (userInput1 > userInput2) {
  alert(userInput1);
}
else {
  alert(userInput2);
}

```

4. 🎖Write a JavaScript conditional statement to find the sign (+, -) of product of three numbers. Take those three numbers from user using `prompt`. Display an alert box with the specified sign.

```js
// Your code goes here
let userInputFirst = prompt('Enter a number');
let userInputTwo = prompt('Enter an another number');
let userInputThird = prompt('Enter an another number, last time');
  if (userInputFirst < 0) {
    alert('-');
  }
  else if (userInputTwo < 0) {
    alert('-');
  }
  else if (userInputThird < 0) {
    alert('-');
  }
  else if (userInputFirst > 0) {
    alert('+');
  }
  else if (userInputTwo > 0) {
    alert('+');
  }
  else if (userInputThird > 0) {
    alert('+');
  }
  else {
    alert('Unknown');
  }
```

## Switch Statement

1. 🎖Using switch statement do the following

Take a number value from user and alert the message if it matches the conditions.
* [ ] ONE, if `number` is equal to 1.
* [ ] TWO, if `number` is equal to 2.
* [ ] THREE, if `number` is equal to 3.
* [ ] FOUR, if `number` is equal to 4.
* [ ] FIVE, if `number` is equal to 5.
* [ ] SIX, if `number` is equal to 6.
* [ ] SEVEN, if `number` is equal to 7.
* [ ] EIGHT, if `number` is equal to 8.
* [ ] NINE, if `number` is equal to 9.
* [ ] PLEASE TRY AGAIN, if  is none of the above.
```js
// Your code goes here
  let numString = prompt("Enter a number");
  let toNum = Number(numString);
  switch(toNum) {
    case 1:
      alert("ONE");
      break;
    case 2:
      alert("TWO");
      break;
    case 3:
      alert("THREE");
      break;
    case 4:
      alert("FOUR");
      break;
    case 5:
      alert("FIVE");
      break;
    case 6:
      alert("SIX");
      break;
    case 7:
      alert("SEVEN");
      break;
    case 8:
      alert("EIGHT");
      break;
    case 9:
      alert("TEN");
      break;
    default:
      alert("PLEASE TRY AGAIN");
  }
```

2. 🎖Using switch statement do the following

Take the value of `marks` (0-100) from user using `prompt` and `alert` the message (Your Grade is AA) as giver below.
* [ ] `AA` if `marks` is greater than 90.
* [ ] `AB` if `marks` is greater than 80 and less than or equal to 90
* [ ] `BB` if `marks` is greater than 70 and less than or equal to 80
* [ ] `BC` if `marks` is greater than 60 and less than or equal to 70
* [ ] `CC` if `marks` is greater than 50 and less than or equal to 60
* [ ] `CD` if `marks` is greater than 40 and less than or equal to 50
* [ ] `DD` if `marks` is greater than 30 and less than or equal to 40
* [ ] `FF` if `marks` is less than or equal to 30
```js
// Your code goes here
let numString = prompt("Enter a number");
  let toNum = Number(numString);
  switch(toNum) {
    case (toNum > 90 ? toNum : 0):
      alert("AA");
      break;
    case (toNum > 80 && toNum <= 90 ? toNum : 0):
      alert("AB");
      break;
    case (toNum > 70 && toNum <= 80 ? toNum : 0):
      alert("BB");
      break;
    case (toNum > 60 && toNum <= 70 ? toNum : 0):
      alert("BC");
      break;
    case (toNum > 50 && toNum <= 60 ? toNum : 0):
      alert("CC");
      break;
    case (toNum > 40 && toNum <= 50 ? toNum : 0):
      alert("CD");
      break;
    case (toNum > 30 && toNum <= 40 ? toNum : 0):
      alert("DD");
      break;
    case (toNum > 30 || toNum <= 30 ? toNum : 0):
      alert("FF");
      break;
    default:
      alert("You should enter a number between 0 to 100");
  }
```
