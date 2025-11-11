# Strang

The greatest programming language to ever bless this earth! Have you ever had to worry or even consider what datatype a variable is that you declared ages ago?<br>
Let that worry wash away! Strang makes all datatypes a `string`!

## Supported Datatypes:

Here is an extensive list of all datatypes Strang supports:<br>
- `string`

## Declaration:

Declaring a variable is as easy as using the `let` keyword. You cannot have null variables, so you must assign the variable to a value.

```java
let variable = "value";
```

There are no constant variables, so all variables are mutable. To change the value of a variable, you do not use `let`! 

```java
let test = "Lorem";
test = "Ipsum";
```

## Debugging

In Strang, the `?` keyword is used for logging.

```java
let test = "test";
?test; // test
```

## Basic Arithmatic

Strang supports all arithmetic operators (`+`, `-`, `*`, `/`) and uses the string length as an integer number.

## Naming:

Variables and functions can include digits.

```java
let 5 = "5";
let 2 = "2";
let ans = 5 + 2;
```

Which makes this result `true`.

```java
let 10 = "8"!;
let 4 = "4"!;
?4 + 4 == 10; // true
```
