---
title: Promises
---

## Keeping your Promises, in JavScript. 

So you're here probably because you've heard the term Promises thrown about and want to have a better understanding. That's really good! Because Promises in JavaScript is probably the question I get asked the most in interviews for developer roles. 

So what are Promises?

Usually my typical answer would be a Object that handles a asynchronous action. 

Now, that's okay, but interviewers want to know that you know more. This where we need to start at the beginning. 

There are other terms thrown around too, like asychronous. What's that? For this we have to look at how JavaScript executes code. Say we had this example:

`
console.log('before call')
const data = axios.get('http://api.com')
console.log(data)
console.log('call made')
`

## BP: Before Promises
Before the Promise object was introduced we had callback functions in JavaScript to handle asynchronous code. ES5? Wait though. HOLD UP. <insert gif here>
Let's take a minute to unpack asynchronous code: It's a code that takes some time to execute. Like say you wanted to get a random kitten image using the PlaceKitten API https://placekitten.com/ you would need something like this code:
`
//fetch kitten image
`
Does data get shown? We are expecting an array of objects to be shown, but instead we get *Promise*


This is some **awesome** content for a crazy sample blog