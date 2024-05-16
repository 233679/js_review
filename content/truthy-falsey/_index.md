+++
title = 'Truthy & Falsey'
+++

So, to explain, as you might have figured from the first example, javascript **is not** strongly typed.
A noteable example of this is what values javascript considered to be "true" or "false". Its definitation is... Loose...

{{< figure src="truthy-falsey.png" title="Truthy-Falsey table!">}}

Looking at the above table. You **will** be confused, so let me explain a little bit.  
The values that javascript *consider* to be true are called "truthy", these are seen on the left side.
This includes such items as 'false' (It's a string since it's quoted!), and *everything that isn't falsey*.  
Falsey values are at least a little bit better, it makes a tiny bit of sense. But then you *might* remember that converting any variable of any type into true or false is, to put it lightly, *a very bad idea*.

[back to the other horrors]({{% relref "../" %}})