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

There are no constant variables, so all variables are mutable. To change the value of a variable, do not use `let`! 

```java
let test = "Lorem";
test = "Ipsum";
```

## Debugging

In Strang, the `?` keyword is used for logging.

```java
let test = "test";
?test; //test
```

The more `?` you use, the more severe the debug log will be.

```java
?"I LOVE STRANG";                //[LOG] I LOVE STRANG
??"WE ALL LOVE STRANG";          //[WARNING] WE ALL LOVE STRANG
???"IT'S POWER IS TOO GREAT!!!"; //[ERROR] IT'S POWER IS TOO GREAT!!!
//                                 thrown 'IT'S POWER IS TOO GREAT!!!'
```

For logs of severity `WARNING` and above, Strang will add info about where the error was found.

```java
01 ??"Where is this problem happening?"
// [WARNING] at line 01
// 'Where is this problem happening?'
```

## Basic Arithmatic

Strang supports all arithmetic operators (`+`, `-`, `*`, `/`) and uses the string length as an integer number. The standard character is `!`.

```java
// Addition
let example = "!!" + "!!!";
?example; // !!!!!
```
```java
// Subtraction
let example = "!!!!!" + "!!";
?example; // !!!
```
```java
// Multiplication
let example = "!!" + "!!!!";
?example; // !!!!!!!!
```
```java
// Division
let example = "!!!!!!" + "!!";
?example; // !!!
```

You can parse a string positive number into a bunch of `!` by putting `!` after the string.

```java
let ten = "10"!;
?ten; // !!!!!!!!!!
```

## Operators

Although the standard character for basic arithmatic is `!` you can still use other characters!

```java
// Multiplication
let laugh = "ha" * "!!!";
?laugh; // hahaha
```

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
?4 + 4 == 10; //true
```
