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


