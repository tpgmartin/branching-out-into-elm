# Laying the Foundations

## The Motivation for Functional Programming

Ask anyone anything about functional programming and in a flurry of words, they might same something about "state", "purity", "functions"", and of course immutability". What does any of this mean? Let's look term by term.

Let's say we load a web page, it has a set of assets including the HTML, CSS, JavaScript, images, and database. If we interact with the page, say toggle a button with a mouse click we are changing the "state" of the web page. Or in other words, the "state" of a web page, is the web page at a particular moment in time. Thinking more abstractly about an application in general, the state is all the set of values that define the application in a given moment. What would be great is for this state to be both **exhaustive** and **reproducible**. This is essentially a guarantee to future-me that I can achieve the present state from any previous state, provided I have a known starting position, and I can reproduce all the steps to get there. Functional programming aims to enshrine this guarantee in code.

How do we make the state precisely reproducible? We need to talk about the terms "purity" and "functions". There's no real mystery to the term "functions": Assuming you've used some programming language you've used a function at some point to return an output on command, often with an input. However, in relation to functional programming languages, functions take on a more precise meaning. We mean something that only ever acts on the given input in a precise and repeatable way. This is what distinguishes a "pure" function, an "impure" on the other hand will change other entities besides its inputs. Impure functions lead to "side-effects", which we'll come to later.

How to make the state exhaustive? This is where "immutability" comes in. We want the entities that are used within the app to be immutable. Instead, when a function is applied to an input, we copy it so we are left with the original copy untouched, and an updated copy with the function applied. Coming full circle, this combination of pure functions and immutable entities ensures that state at any point in time is both exhaustive and reproducible: the state is precisely the result of an immutable past.

## Thinking in Functions



## Chapter in Review
