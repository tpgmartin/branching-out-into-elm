# Laying the Foundations

## The Motivation for Functional Programming

Ask anyone anything about functional programming and in a flurry of words, they might same something about "state", "immutability", "purity", and of course "functions". What does any of this mean? Let's look term by term.

Let's say we load a web page, it has a set of assets including the HTML, CSS, JavaScript, images, and database. If we interact with the page, say toggle a button with a mouse click we are changing the "state" of the web page. Or in other words, the "state" of a web page, is the web page at a particular moment in time. Thinking more abstractly about an application in general, the state is all the set of values that define the application in a given moment. What would be great is for this state to be both **exhaustive** and **reproducible**. This is essentially a guarantee to future-me that I can achieve the present state from any previous state, provided I have a known starting position, and I can reproduce all the steps to get there. Functional programming aims to enshrine this guarantee in code.

This is where immutability comes in. We want the state to be immutable, at least for any given moment in time. 

## Chapter in Review
