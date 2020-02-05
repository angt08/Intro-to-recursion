# Recursion
<details>
<summary>
    Hi,welcome to RECURSION:
  </summary>
</summary>
<details>
  <summary>
    Hi,welcome to RECURSION:
  </summary>

![](https://media.giphy.com/media/12ZDIx1Mw1cXVm/giphy.gif)

  ***Recursion***: In it's simplest form is a function which calls itself like so
  >
  ```
  
  function iAmCallingMyself(){

	iAmCallingMyself()
	
}
 iAmCallingMyself() //--> If you Run this example you will get an error, Don't do it.

  ```

 >
 If you do run this code example, this is the error message you will encounter:  
 > ![](https://i.imgur.com/IRRQr5F.png?1)
 This error is what's known as **Stack Overflow**
 >
#### WAIT! Before we dive into Recursion let's first define the Call Stack
 >
***Call Stack***: 
Is a small data structure 
which keeps track of functions being called.
The call stack keeps track of these function calls one by one, top to bottom. 
>
At the end of a function call and execution, the call stack pops off the function that just executed 
and pushes in the next function. 
>
The call stack holds these functions along with their variables, conditions and other parameters you've implemented,  
this creates a small stack frame within it's memory.
So imagine how running a function which calls itself with no end(**base case**)will eventually 
take up the maximum stack call resulting in a **Stack Overflow**. 

![](https://media.giphy.com/media/3ohs4rkYvzISB83cqY/giphy.gif)
>
>[Note: Reference code and super useful article for above gif here.](https://frontend.turing.io/lessons/module-2/scope-1.html)

>   
#### Now that we have a swift idea of what the call stack is and keeping in mind it's duties
#### let's get back to Recursion
![](https://pics.me.me/thumb_now-lets-see-who-you-really-are-recursion-now-lets-44360522.png)

#### What is it?
>
We know Recursive functions are functions that call themselves, 
but why would we want a function to do this?
>
Well Functions are reusable blocks of code, 
you can make functions iterate multiple elements within it,
>
so for example rather than making multiple if/else statements, or multiple loops, 
you could write a function that manipulates data elements within it's scope,
with a recursive function this can be done multiple times
hence your code will be cleaner and easier to read. 
>

Example code with NO recursion:
```
function notARecursiveFunction(num) {

 for (let i = num; i >= 1; i--) {
   console.log(i);
 }
}
notARecursiveFunction(10);//--> output will be 10,9,8,7,6,5,4,3,2,1
```
>

Example code with Recursive approach:
```
let countDown = 10;

function theFinalCountDown( ){
	if (countDown === 0)//--> this is your base case to break out of this recursive function
    return 'count down ends here'
    countDown --;

	console.log(countDown)

    return theFinalCountDown()
} 

theFinalCountDown()//--> output:9,8,7,6,5,4,3,2,1,0,'count down ends here'


```
>
Mentioned above is **Base Case** this is essential when writing your recursive function,
why? well a recursive function will call itself indefinitely, the base case is it's stop point. 
It is what will break this Recursive function call. Don't forget to give your recursive functions base case or your computer  will die. 

  

    
</summary>
</details>
</details>


### What du heck
