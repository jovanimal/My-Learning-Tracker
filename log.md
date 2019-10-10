# Learning log

|Date |                                        |
|:---:|:---------------------------------------|
|     |Progress, thoughts and ideas	       |

## Full [Log Index]

[__************** 2019 Objectives **************__]

----------------------------------------------------------

----------------------------------------------------------
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


