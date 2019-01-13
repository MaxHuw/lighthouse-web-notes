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
"中文 español Deutsch English देवनागरी العربية português বাংলা русский 日本語 norsk bokmål ਪੰਜਾਬੀ 한국어 தமிழ் עברית"


```
##### Escape Notation

Besides regular, printable characters, special characters can be encoded using escape notation:

```javascript
\'      Single Quote
\"      Double Quote
\\      Backslash
\n      New Line
\r      Carriage Return
\v      Vertical Tab
\t      Tab
\b      Backspace
```

#### Symbol

Symbols are new to JavaScript in ECMAScript 2015. A Symbol is a unique and immutable primitive value and may be used as the key of an Object property (see below). In some programming languages, Symbols are called atoms. For more details see Symbol and the Symbol object wrapper in JavaScript.

### Onjects

In JavaScript, objects can be seen as a collection of properties. With the object literal syntax, a limited set of properties are initialized; then properties can be added and removed. Property values can be values of any type, including other objects, which enables building complex data structures. Properties are identified using key values. A key value is either a String or a Symbol value.





```javascript

function whatToDoForLunch(hungry, availableTime) {
  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
}

```