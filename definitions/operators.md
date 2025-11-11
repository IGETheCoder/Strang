# All Operators

## '*Int*'eger

Strang itself doesn't support the _'int'_ datatype, but there are still some _'int'_ operators that use the string length instead.
 - `"9"!` **Int Parse**
 ```java
?"6"!; //!!!!!! 
 ```
 Strang first parses the positive numeric string, and creates a new string with _n_ length of `!`.<br>
 The `!` is the standard character for arithmatic in Strang.
- `"target"["!!"]` **Char Of**
 ```java
?"apple"["!!!"]; //l
 ```
 Find's the character of a _target_ string, that is _n length_ distance from the origin.

## String Manipulation

Strang offers plenty of operators for string manipulation, built straight in.
 - `#` **Interweave**:
 ```java
?"abc" # "xy"; //axaybxbycxcy
 ```
 Inspired by mathmetics: iteratively takes the first character from `stringA` and concatanates it with the first character from `stringB`. Then the second character from `stringA` so on ... (`stringA` is left, `stringB` is right)<br>
 Makes the length of the string `a * b * 2`
 - `^` , `^^` **To Lower** _and_ **To Upper**:
 ```java
?"HIGH"^; //high
?"low"^^; //LOW
 ```
 Converts all the letters from the _target_ string to lowercase or to uppercase, depending on the operator used.
 - `--` , `---` **Remove Substring** _and_ **Remove Characters**:
 ```java
?"hello world" -- "lo";  //hel world
?"hello world" --- "lo"; //he wrd
 ```
 Removes all the matches from _target_, based on the _pattern_ (case sensitive):
   - Remove Substring will remove all the text from the _target_, if they match the string, letter for letter.
   - Remove Characters will remove any character that is from the _pattern_
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

## '*Bool*'ean Operators

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

### Why stop there?

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

## Relational Operators

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

## Extra Operators

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
