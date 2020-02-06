# Recursion
<details>
<summary>
    Hi,welcome to RECURSION:
  </summary 
</summary>
	
<details>
   <summary>
    Hi,welcome to RECURSION:
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
 >
 This error is what's known as **Stack Overflow**
 >
#### WAIT! Before we dive into Recursion let's first define the Call Stack
 >
**Call Stack**: 
Is a small data structure 
which keeps track of functions being called.
The call stack keeps track of these function calls one by one, top to bottom. 
>
At the end of a function call and execution, the call stack pops off the function that just executed after a **Return** value is given and pushes in the next function  
>
The call stack holds these functions along with their variables,conditions and other parameters you've implemented,  
this creates a small stack frame within it's memory.
So running a function which calls itself with no end(**base case**)
will eventually take up the maximum stack call resulting in a **Stack Overflow**. 

![](https://media.giphy.com/media/3ohs4rkYvzISB83cqY/giphy.gif)
>
>[Note: Super useful article for above gif here.](https://frontend.turing.io/lessons/module-2/scope-1.html)

>   
#### Now that we have a swift idea of what the call stack is and keeping in mind it's duties
#### Great,now back to Recursion:
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
with a recursive function this can be done multiple times. 
Your recursive function will need two things, a **base case** or exit point, 
and a **recursive case** case which is just the function calling itself.
>
Recursive functions  break up bigger problems into smaller blocks
hence your code will look cleaner and easier to read.

> believe it or not, recursive functions, though efficient and crafty,
are not your end all be all, so don't think you have to code them for everything you write in programming.

>

Example code with NO recursion:
```

function notARecursiveFunction(num) {

 for (let i = num; i >= 1; i--) {
   console.log(i);
  }
}
notARecursiveFunction(10); //--> output: 10,9,8,7,6,5,4,3,2,1
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

    return theFinalCountDown()--> this is your recursive case in this function, here we have the fucntion calling itself.
} 

theFinalCountDown()//--> output: 9,8,7,6,5,4,3,2,1,0,'count down ends here'

```
>
Mentioned above is **Base Case** this is essential when writing your recursive function,
why? Well a recursive function will call itself indefinitely, the base case is the stop point,this returns a value. 
Your base case is what will break/end a Recursive function call.
Do not forget to give your recursive functions a base case or your computer  will die. 



Now some more examples of this phenomenon
```


```
>
#### let's recap what the heck were we introduced to?
>
#### Recursive Functions:
>
- A function that calls itself
- Is composed of a recursive case and a base case.
>
- If you  don't give your recursive function a base case your computer....will perish. 
- Is great for big problems and breakin them down into smaller blocks.
>
##### Call Stack:
>
- The call stack holds these fucntions in its block of memory , creating a stack frame for each one.
- The call stack can only track one function at a time from top to bottom.
- When a value is returned from a function, the call stack pops off that function and pushed in a new one.
>
#### [Hands on practice](https://git.generalassemb.ly/sei-nyc-blizzard/recursion-practice/blob/master/recursion.js)

Still don't full understand? that's okay, even most seasoned programmers 
have difficulty wrapping their heads around recursive functions,
just ask them
in the meantime check these out. 
>
[Recursion video 13min](https://youtu.be/6oDQaB2one8)
>

</summary>   
</details>
</details>

### What du heck
