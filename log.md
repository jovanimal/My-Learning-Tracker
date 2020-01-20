# Learning log

|Date |                                        |
|:---:|:---------------------------------------|
|     |Progress, thoughts and ideas	       |

## Full [Log Index]
[__************** 2020 Objectives **************__]

----------------------------------------------------------
To fast track my learning by building projects and eventually get into a full time tech role.

----------------------------------------------------------


[__************** 2019 Objectives **************__]

----------------------------------------------------------
To build up my foundation in front end web development, particularly Javascript and JS frameworks.

----------------------------------------------------------
## Mon 20 Jan 20
Second week into the coding bootcamp !

## Fri 17 Jan 20
Second day into Javascript, introducing loops (e.g For, while, if statement). The group activity is a challenging one as our group got the hardest problem (claimed by the mentors), and we are only allowed to use ONE while loop. We went through stack overflow and found a similar solution but we didn't understand what the code says. Thus we re-engineer and break it down into pieces and we got it after half an hour. Solution:

```
function romanize(num) {
  if (isNaN(num))
    return NaN;

  let digits = String(num).split("");

  const key = ["", "I", "II", "III", "IV", "V", "VI", "VII", "VIII", "IX",
    "", "X", "XX", "XXX", "XL", "L", "LX", "LXX", "LXXX", "XC",
    "", "C", "CC", "CCC", "CD", "D", "DC", "DCC", "DCCC", "CM",
    "", "M"];

  let roman = "";
  
  let i = 0; 
  while (i < num.length) {
    roman = (key[+digits.pop() + (i * 10)]) + roman; 
    i ++}

  return roman;
  
}

console.log(romanize(1426));
```

## Thu 16 Jan 20

First day of JavaScript, I'm like "YESS, finally!" Nothing particularly challenging as I've been writing JS for 4 months now. Group presentation on explaining data prototypes, e.g. push, indexOf, sort, includes etc. First Challenge is to use write javascript so that it will calculate your BMI for you: https://code.nextacademy.com/lessons/exercise--bmi-calculator/980. I wrote it in a function since it can take in both parameters: 

```
function calculateBMI(myWeight, myHeight) {
  let myBMI = myWeight / (myHeight * myHeight);
  if (myBMI < 18.5) console.log(`Your BMI is ${myBMI}. You are underweight`);
  else if (myBMI >= 18.5 && myBMI <= 24.9)
    console.log(`Your BMI is ${myBMI}. You are in the healthy weight range`);
  else if (myBMI >= 30 && myBMI <= 40)
    console.log(`Your BMI is ${myBMI}. You are overweight`);
  else console.log("Why my BMI is not specified!!!");
}

calculateBMI(82, 1.78); //  return Why my BMI is not specified!!!

```
The second challenge is FizzBuzz: https://code.nextacademy.com/lessons/challenge--fizzbuzz/868 -
```
<!DOCTYPE html>
<html>
  <body>
    <p>Click the button to demonstrate the fizzBuzz.</p>

    <button onclick="fizzBuzz()">Try it</button>

    <p id="demo"></p>

    <script>
      function fizzBuzz() {
        let number = prompt("Please enter your number");
        let result = "";
        if (number >= 1 && number <= 100) {
          if (number % 3 == 0 && number % 5 == 0) {
            alert("FizzBuzz");
          } else if (number % 3 == 0) {
            alert("Fizz");
          } else if (number % 5 == 0) {
            alert("Buzz");
          }
        } else alert("Enter a number between 1-100!");
      }
    </script>
  </body>
</html>
```

## Wed 15 Jan 20

Working on Bootstrap. First Challenge is to use only Bootsrap to clone a website without writing any CSS code: https://bootstrap-next-example.netlify.com/. Though I have limited experience on Bootstrap, it's impressive to see what Bootstrap alone can do and I get to know Bootstrap in an in-depth level today. Good stuff.

The second challenge is to use a combination of Bootstrap and CSS to clone a website: https://musing-goodall-f54def.netlify.com/.

## Tue 14 Jan 20

Mainly working on CSS Animations. We have a group project after lunch which requires us to clone a website: https://shopme-next.netlify.com/. Worked with team member Kay Shaun and Irsyad.

Materials on flexbox to read:

1. https://flexboxfroggy.com/
2. https://css-tricks.com/snippets/css/a-guide-to-flexbox/
3. https://github.com/samanthaming/Flexbox30#align-items-row

## Mon 13 Jan 20

First day of Next Academy Full Stack Web Development Bootcamp. Introduction to HTML & CSS, refershing what I have gone through on FreeCodeCamp and Codecademy when I first started coding in Sept 2019. 

## Wed 30 Oct 19

Completed a [HackerRank](https://www.hackerrank.com/) algorithm which move the first ```n``` element in an array to the back of the array.

```
function shiftLeftNumber (arr,n) {
  for (i = 1; i <= n; i++) {
  arr.push(arr.shift ());
  }
  console.log(arr)
}

shiftLeftNumber([1,2,3,4,5,6,7],2)
// → return [ 3, 4, 5, 6, 7, 1, 2 ]
```

## Tue 22 Oct 19

Completed 3 exercises from [Eloquent JavaScript](http://eloquentjavascript.net/) without looking at the hints and got it all right ! Confidence boosted ! :)

Bean counting:

```
function countBs (text) {
  return countChar(text, "B");
}

function countChar (phrase, n) {
  let count = 0;
  for (let i = 0; i < phrase.length; i++) {
    if (phrase[i] === n) {
      count += 1;
    }
  }
  return count;
}
console.log(countBs("BBC"));
// → 2
console.log(countChar("kakkerlak", "k"));
// → 4
```

## Fri 11 Oct 19

Completed a chess game today from [Eloquent JavaScript](http://eloquentjavascript.net/).

```
let size = 10;

let board = "";

for (let y = 0; y < size; y++) {
  for (let x = 0; x < size; x++) {
    if ((x + y) % 2 == 0) {
      board += " ";
    } else {
      board += "#";
    }
  }
  board += "\n";
}
console.log(board);

//output:
 # # # # #
# # # # # 
 # # # # #
# # # # # 
 # # # # #
# # # # # 
 # # # # #
# # # # # 
 # # # # #
# # # # # 
```

## Thu 10 Oct 19

Completed [Intro to HTML & CSS](https://www.udacity.com/course/intro-to-html-and-css--ud001) from Udacity.

## Mon 7 Oct 19

Weekly Coding Group, HiPo coding Group learning today:
Usage of Digital Ocean for cloud services and Caddy.

## Sat 5 Oct 19

Finished reading [YDKJS: Getting Started](https://github.com/getify/You-Dont-Know-JS/blob/2nd-ed/getting-started/README.md).

## Thu 3 Oct 19

While reading [You Don't Know JavaScript](https://github.com/getify/You-Dont-Know-JS/blob/2nd-ed/getting-started/ch2.md), important note on **Nested Scopes**:

When you declare a variable, it is available anywhere in that scope, as well as any lower/inner scopes. However, you have no access to variable declared in a inner scope from outer level.

```
function foo() {
	var a = 1;
  
	function bar() {
		var b = 2;

		function baz() {
			var c = 3;

			console.log( a, b, c );	// 1 2 3
		}

		baz();
		console.log( a, b );		// 1 2
	}

	bar();
	console.log( a );				// 1
}

foo();
```


