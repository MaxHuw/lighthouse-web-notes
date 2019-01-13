# JavaScript Cheatsheet

## Table of Contents

* [Data Types](##data-types)
  * [Primatives](###primatives)
    * [Boolean](###Boolean)
    * [Null](###Null)
    * [Undefined](###Undefined)
    * [Number](###Number)
    * [String](###String)
    * [Symbol](###Symbol)

## Data Types

### Primatives

#### Boolean

Boolean represents a logical entity and can have two values: true, and false.

#### Null

The Null type has exactly one value: null. See null and Null for more details.

#### Undefined

A variable that has not been assigned a value has the value undefined. See undefined and Undefined for more details.

#### Number

There is no specific type for integers. In addition to being able to represent floating-point numbers, the number type has three symbolic values: +Infinity, -Infinity, and NaN (not-a-number).

#### String

JavaScript's String type is used to represent textual data. It is a set of "elements" of 16-bit unsigned integer values. Each element in the String occupies a position in the String. The first element is at index 0, the next at index 1, and so on. The length of a String is the number of elements in it.

Unlike in languages like C, JavaScript strings are immutable. This means that once a string is created, it is not possible to modify it. However, it is still possible to create another string based on an operation on the original string. For example:

A substring of the original by picking individual letters or using String.substr().
A concatenation of two strings using the concatenation operator (+) or String.concat().

##### Examples

```javascript

'string text'
"string text"
"中文 español Deutsch English देवनागरी العربية português বাংলা"

```

Besides regular, printable characters, special characters can be encoded using escape notation:

```javascript
\'      //Single Quote
\"      //Double Quote
\\      //Backslash
\n      //New Line
\r      //Carriage Return
\v      //Vertical Tab
\t      //Tab
\b      //Backspace
```

You can concatonate strings together with the + operator.
```javascript
let longString = "This is a very long string which needs " +
                 "to wrap across multiple lines because " +
                 "otherwise my code is unreadable.";
```

##### String Methods

##### Accessing Characters

There are two ways to access an individual character in a string. The first is the charAt() method:

```javascript
return 'cat'.charAt(1); // returns "a"
```

The other way (introduced in ECMAScript 5) is to treat the string as an array-like object, where individual characters correspond to a numerical index:

```javascript
return 'cat'[1]; // returns "a"
```

##### Finding Length of String

```javascript
var browserType = 'mozilla';
browserType.length; // = 7
```

##### Finding a substring inside a string and extracting it

```javascript
browserType.indexOf('zilla'); // = 2 (the index of where substring starts)

browserType.indexOf('vanilla'); // = -1, because the substring is not in it.
```
##### Slice()

Returns a section of a string.

```javascript
browserType.slice(0,3);

//Returns 'moz'. First param is start of new substring, and second is the
//character after the end of the sub string. Leave the second param blank to
// return the rest of the string.

browserType.slice(2) //Returns 'zilla'
```

##### Changing Case

Can change the characters in a string to Upper or Lower case.
```javascript
var radData = 'My NaMe Is MuD';
radData.toLowerCase(); // 'my name is mud'
radData.toUpperCase(); // 'MY NAME IS MUD'
```

##### Updating Part of a String

You can replace one substring inside a string with replace(). It takes two parameters, the substring you want to replace, and the string you want to replace it with.

```javascript
browserType.replace('moz','van'); // Returns 'vanilla'
```
Note: To actually update the value of browserType, you need to set it to be the result of the opperator. ex:

```javascript
browserType = browserType.replace('moz','van');
```




For character access using bracket notation, attempting to delete or assign a value to these properties will not succeed. The properties involved are neither writable nor configurable.

#### Symbol

Symbols are new to JavaScript in ECMAScript 2015. A Symbol is a unique and immutable primitive value and may be used as the key of an Object property (see below). In some programming languages, Symbols are called atoms. For more details see Symbol and the Symbol object wrapper in JavaScript.

### Objects

In JavaScript, objects can be seen as a collection of properties. With the object literal syntax, a limited set of properties are initialized; then properties can be added and removed. Property values can be values of any type, including other objects, which enables building complex data structures. Properties are identified using key values. A key value is either a String or a Symbol value.





```javascript

function whatToDoForLunch(hungry, availableTime) {
  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
}

```