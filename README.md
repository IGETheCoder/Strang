# Strang

The greatest programming language to ever bless this Earth!<br><br>
Have you ever had to worry, or even consider what datatype a variable is that you declared decades ago? Let that worry _wash away_! Strang makes all datatypes `string`!<br><br>
This programming language is the closest you can get to perfection in the world!!<br><br>

## Table Of Contents:
- [Supported Datatypes](#supported-datatypes)
- [Declaration](#declaration)
- [Debugging](#debugging)
- [String Literals](#string-literals)
- [Basic Arithmatic](#basic-arithmatic)
- [Basic Operators](#basic-operators)
- [Naming](#naming)
- [Operators](#operators)
- [Selection](#selection)
- [Loops](#loops)
- [Functions](#functions)
- [Conclusion](#conclusion)

## Supported Datatypes:

Here is an extensive list of all datatypes Strang supports:<br>
- `string`

The very mention of other datatypes will make `string` jealous, so I will _'whisper'_ other datatypes.

## Declaration:

Declaring a variable is as easy as using the `let` keyword. You cannot have _'null'_ variables, so you must assign the variable to a value.

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

Why use ``var `=``? It's actually a simple way for declaring string variables of zero length!
```
let empty `=;
?empty; //
```

If you want to define a string using ``var `=`` and have the variable start with whitespace, put a `\` and Strang will omit all whitespace up to that point.
```
let string `= \     SO MUCH WHITESPACE;
?string; //     SO MUCH WHITESPACE
```

## Basic Arithmatic

Strang supports all arithmetic operators (`+`, `-`, `*`, `/`) and uses the string length as an _'integer'_ value. The standard character is `!`.

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

Check out all the operator definitions [here](https://github.com/IGETheCoder/Strang/blob/main/definitions/operators.md)!

### '*Int*'eger

Strang itself doesn't support the _'int'_ datatype, but there are still some _'int'_ operators that use the string length instead.
 - `"9"!` **Int Parse**
 ```java
?"6"!; //!!!!!! 
 ```
- `"target"["!!"]` **Char Of**
 ```java
?"apple"["!!!"]; //l
 ```

### String Manipulation

Strang offers plenty of operators for string manipulation, built straight in.
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

### '*Bool*'ean Operators

Strang doesn't support the _'boolean'_ datatype, so Strang uses string literals of `"true"` _and_ `"false"`.<br>
Unlike most programming lanuages, Strang much prefers to use, beautiful, juicy words instead of _grotesque symbols._

 - `AND`
 - `OR`
 - `XOR`
 - `XAND`

But we like `!` to be 'not' instead of `NOT`. Why? i dont know.

```java
let bobobolo = !"true";
?bobobolo; //false
```

If you use a _'boolean'_ operator on a non-_'boolean'_ string, such as `TRUTH`, instead of throwing, we follow what the best of the best do.<br>
`maybe`

```java
let what = !"TRUTH";
?what; //maybe
```

#### Why stop there?

If you try performing _'boolean'_ operators on `maybe`, you get:
```java
?!"maybe"; //possibly
```

This doesn't stop at `possibly`! Just like Strang!

```java
?!"maybe"; //possibly
?!"possibly"; //probably
?!"probably"; //probably not
?!"probably not"; //quite frankly
?!"quite frankly"; //could potentially
?!"could potentially"; //okay this is the last one
```

Who said you could stop at that!

```java
?!"okay this is the last one"; //i lied
```

### Relational Operators

- `==` **Equals** (not length)
```java
?"apple" == "apple"; //true
?"apple" == "zebra"; //false
```
- `!=` **Not Equals** (not length)
```java
?"apple" != "apple"; //false
?"apple" != "zebra"; //true
```
- `<` , `>` **Less Than** _and_ **Greater Than** (length)
```java
?"banana" > "apple"; //true
?"5"! < "8"!;        //true
```
- `<=` , `>=` **(Less Than** _and_ **Greater Than) Or Equals** (length)
```java
?"3"! > "3"!;  //false
?"3"! >= "3"!; //true
```

### Extra Operators

- `<<` , `>>` **Starts With** _and_ **Ends With**
```java
?"banana" << "ba"; //true
?"banana" >> "ba"; //false
?"banana" >> "na"; //true
```
- `~` **Contains**
```java
?"hello world" ~ "lo"; //true
?"apple" ~ "z"; //false
```

## Selection

Strang has the `if` , `if...else` and `if...else if` keywords for selection, and expect the conditional to be `"true"` or `"false"`.

```java
if ("5"! > "2"!)
{
    ?"5 is bigger than 2!";
}
else
{
    ???"how did you manage that";
}
```

If Strang gets a non-_'boolean'_ string, it will throw. I was considering adding another keyword, like `grasp` to use for non-'*boolean*'s, and it will probably be implemented in the close future!

## Loops

In Strang, the `for` loop doesn't exist. Our beloved `string` hates that guy. Instead we have the replacement `foreach`.<br>
`foreach` loops through each individual character, and declares the character you currently index at.

```java
let target = "test";
foreach (let c in target)
{
    ?c;
}
```
```
//t
//e
//s
//t
```

We also have `while`, which acts similiarlly to `if`, except it loops. Like most programming languages...

```java
while ("true")
{
    ?"BEWARE THE MAN WHO SPEAKS IN HANDS";
}
```

_i dont think i needed to explain that_

## Functions

Functions are declared using either of these keywords: `func` , `funcstr`<br>
<br>
`func` doesn't expect a return value,<br>
`funcstr` does expect a return value.

```java
func Test()
{
    ?"you called?";
}
```
```java
funcstr Destroy()
{
    return "so you have chosen death...";
}
```
When declaring a function, the function arguments must have the `let` keyword for each argument.

```java
funcstr Concat(let a, let b)
{
    return a + ' ' + b;
}
```

Calling the function is as simple as `FunctionName()` or if the function has arguments,

``` java
?Concat("Hello","World");
```

## Conclusion

The best language ever! You should use it for your everyday programming! Convince your boss to switch to Strang now!
