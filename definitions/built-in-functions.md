# Built-In Functions

[Go Back](https://github.com/IGETheCoder/Strang/blob/main/README.md)

## Table Of Contents
 - [Lorem Ipsum](#lorem-ipsum)

## Lorem Ipsum

`LoremIpsum()` By default, expects no parameters, but can be provided with an optional `length` parameter.

```java
?LoremIpsum(); //Lorem ipsum.
```

`LoremIpsum(length)` The first parameter corrisponds with how many words that will be generated. The generator uses randomness to determine what word to produce

```java
?LoremIpsum("10"!); //Lorem ipsum magna bibendum cras massa lacinia integer sociosqu scelerisque.
```

## Length

`Length(target)` Expects one parameter as a target string. It will output the length of the string as a string numeric.

```java
?Length("apple"); //5
```
```java
?Length("banana"); //6
```
```java
?Length("200"!); //200
```

## Reverse

`Reverse(target)` Expects one parameter as a target string. It will output the string in reverse order.

```java
?Length("Apple"); //elppA
```
```java
?Length("Lorem"); //meroL
```

## ReadLine

`ReadLine()` Expects no parameter. It will wait until the user inputs a string value, then output that.

```java
?"Enter your name: ";
let input = ReadLine();
?"Your name is " + input;
```

## Write

`Write(text)` Expects one parameter as a text string. It will display the text to the console, but without a line break at the end.

```java
Write("hello ");
Write("world");
```
```
//hello world
```

## WriteLine

`WriteLine(text)` Expects one parameter as a text string. It will display the text to the console, with a line break at the end. Functionally same to `?` debug keyword.

```java
WriteLine("hello");
WriteLine("world");
```
```
//hello
//world
```

## Random

`Random(min, max)` Expects two parameters as min length and max length. It will output a random amount of `!` between min and max. If min is bigger than max, it is automatically switched.

```java
?Random("1"!, "10"!); //random amount from 1-10
```
```
//!!
//!!!!!!
//!!!!
//!!!!!!!!!
```

## ToTitleCase

`ToTitleCase(input)` Expects one parameter as an input string. It will output the input string, but with the first character capitalized.

```java
?ToTitleCase("hello"); //Hello
```
```java
?ToTitleCase("apple"); //Apple
```

## Finished?

You can [Go Back](https://github.com/IGETheCoder/Strang/blob/main/README.md)
