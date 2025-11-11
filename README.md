# Strang

The greatest programming language to ever bless this Earth! Have you ever had to worry or even consider what datatype a variable is that you declared ages ago?<br>
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
// thrown 'IT'S POWER IS TOO GREAT!!!'
```

For logs of severity `WARNING` and above, Strang will add info about where the error was found.

```java
01 ??"Where is this problem happening?"
// [WARNING] at line 01
// 'Where is this problem happening?'
```

## String Literals:

Most programming languages define strings using `"` quote marks. Some with `'` single quote marks. In Strang, you can use any amount of quotation marks, as long as if the start and end quotes add up the same.
```
'LEGAL'
""LEGAL""
''''LEGAL""
""''"'LEGAL"''"'"
```
 - But if the amout of quotes are mismatched, it is an illegal string definition.
```
"ILLEGAL'
"ILLEGAL"'
```

Even no quotation marks! But only when assigning to a variable. All whitespace before the first character are ommited.
```
let string `= I HAVE NO STRINGS ON ME!;
?string; //I HAVE NO STRINGS ON ME!
```

Why use this? It's actually a very clear way for declaring string variables of zero length!
```
let empty `=;
?empty; //
```

If you want to define a string using ```var `=``` and have the variable start with whitespace, put a `\` and Strang will omit all whitespace up to that point.
```
let string `= \     SO MUCH WHITESPACE;
?string; //     SO MUCH WHITESPACE
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

## Basic Operators

Although the standard character for basic arithmatic is `!` you can still use other characters!

```java
// Multiplication
let laugh = "ha" * "123";
?laugh; //hahaha
```
```java
// Division
let example = "abcdef" / "AB";
?example; //abc
```
```java
// Addition
let hallo = "Hello " + "World";
?hallo; //Hello World
```

Subtraction has 2 variants. The default is `>-`.<br>
 - `>-` Trim End
 - `-<` Trim Start

```java
// Subtraction (same as >-)
let subtract = "abcde" - "!!";
?subtract //abc
```
```java
// Trim End
let trimEnd = "HELP ME" >- "!!!";
?trimEnd //HELP
```
```java
// Trim Start
let trimStart = "Strang, not C Is Goated" -< "!!!!!!!!!!!!";
?trimStart //C Is Goated
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

## Operators:

Check out all the operator definitions [here]()!

### Integer

Strang itself doesn't support integers, but there are some int operators
 - `"9"!` **Int Parse**
 ```java
?"6"!; //!!!!!! 
 ```
- `"target"["!!"]` **Char Of**
 ```java
?"apple"["!!!"]; //l
 ```

### String Manipulation

Strang offers plenty of operators for string manipulation, built straight in!
 - `#` **Interweave**:
 ```java
?"abc" # "xy"; //axaybxbycxcy
 ```
 - `^` , `^^` **To Lower** _and_ **To Upper**:
 ```java
?"HIGH"^; //high
?"low"^^; //LOW
 ```
 - `--` , `---` **Remove Substring** _and_ **Remove Characters**:
 ```java
?"hello world" -- "lo";  //hel world
?"hello world" --- "lo"; //he wrd
 ```
- `>-` , `-<` **Trim End** _and_ **Trim Start**:
 ```java
?"abcde" >- "!!";  //abc
?"abcde" -< "!!";  //cde
 ```
- `%` **Truncate**:
 ```java
?"ABCDEFGHIJKLMNOP" % "GHI";  //ABCDEF
?"3.14159265" % "15";  //3.14
 ```
