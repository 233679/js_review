+++
title = 'Object.is'
+++

Like many languages, javascript has mutiple ways to compare if two values are the same. It's a bit weird to me but fair enough. 
The problem really starts when these methods produce **different** results. This is the issue between `Object.is()` & `===` in javascript.

### Firstly
```javascript
NaN === NaN; // -> false
Object.is(NaN, NaN); // -> true
```
Credit where credit is due. `===` is giving the correct output (IEEE specifies that NaN != NaN).
Then you see `Object.is()`... Need i say more?  

And these, i'll spare you me ranting about it all..
```javascript
Object.is(-0, 0); // -> false
-0 === 0; // -> true

Object.is(NaN, 0 / 0); // -> true
NaN === 0 / 0; // -> false
```
  
[return to depleeting sanity]({{% relref "../" %}})