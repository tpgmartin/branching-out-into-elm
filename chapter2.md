# Elm Fundamentals

This section is current as of Elm 0.17

## Overview

In this section, we will cover
* Elm tooling
* Elm syntax
* Modules
* Elm functions
* Currying
* Composition
* Elm types
* Functors
* The Elm architecture

## Elm Functions

At long last, we get to look at Elm functions! Elm supports prefix and infix functions. In either case, the syntax is very clean and minimalist. For instance a simple add function can be written as,

```
add a b =
  a + b
```

where, the function name is at the top left, the parameters follow in a space separated by spaces. The beginning of the function body is indicated with "=" followed by the expression to be returned. No explicit return statement is required.



## The Elm Architecture

The Elm Architecture refers to a design pattern common to Elm apps, which has been heavily emphasised as of the 0.17 release. This pattern is to split code into the Model, Update, and View functions, and Action types. The Elm Architecture is also referred to as the "Model View Update" for this reason.

Peculiar to this pattern is the universal composition of each function and type mentioned specification: Views can be composed of nested views, Models of nested models etc. As a consequence, Elm components or UI element must consistently posses Model (with an initial Model), View, Update functions, and an Action type.

(Add diagram here)

These three components communicate in a unidirectional manner, as previously discussed.

This is such a common pattern, that it is strongly advised to use [starter skeleton](https://github.com/evancz/elm-architecture-tutorial/) for any new project.

For larger apps, the modular path that Elm guides us down via the Elm architecture and, more generally, good functional programming principles gives us a maintainable app for free. We needn't worry about anything else, as <Get citation from podcast>

## Summary