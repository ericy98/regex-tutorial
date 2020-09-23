# Matching a Hex Value

This brief tutorial will explain the validation process for a hex value.

## Summary

I'm going to break down how we can take this regex ```/^#?([a-f0-9]{6}|[a-f0-9]{3})$/``` and how it goes about matching a hex value.

## Table of Contents

- [Matching a Hex Value](#matching-a-hex-value)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
    - [Anchors](#anchors)
    - [Quantifiers](#quantifiers)
    - [OR Operator](#or-operator)
    - [Character Classes](#character-classes)
    - [Flags](#flags)
    - [Grouping and Capturing](#grouping-and-capturing)
    - [Bracket Expressions](#bracket-expressions)
    - [Greedy and Lazy Match](#greedy-and-lazy-match)
    - [Boundaries](#boundaries)
    - [Back-references](#back-references)
    - [Look-ahead and Look-behind](#look-ahead-and-look-behind)
  - [Author](#author)

## Regex Components
```/^#?([a-f0-9]{6}|[a-f0-9]{3})$/```
### Anchors
* The beginning anchor ```^```  signifies the start of the string. The regex will look to see if the string begins with ```#```.
* The end anchor ```$``` checks if the string ends in a number.
### Quantifiers
*  The ```?``` quanitfier matches a string based on whatever values are followed. This regex matches a string that is either followed by 6 values or 3 giving a hex value.
### OR Operator
* The ```|``` operator accepts a hex value of  ```[a-f0-9]{6}``` OR ```[a-f0-9]{3}```
* The ```[]``` operator only accepts whatever string is contained within the brackets.
* The regex accepts a string ```#``` followed by ```[a-f0-9]``` OR ```[a-f0-9]```
### Character Classes
* This regex does not contain any character classes.
### Flags
* This regex does not contain any flags.
### Grouping and Capturing
* ```()``` create a capturing group that only looks at the values within the parenthesis.
* This regex looks to seee if a string matches the capturing group ```([a-f0-9]{6}|[a-f0-9]{3})```
### Bracket Expressions
* ```[]``` matches any string inside. 
* This regex matches a string ```[a-f0-9]```. It must contain any letter from A to F, and/or any number from 0 to 9.
### Greedy and Lazy Match
* Each string must contain either 6 or 3 matching values.
* ```{6}``` of ```[a-f0-9]``` or ```{3}``` of ```[a-f0-9]```
### Boundaries
* There are no boundaries within this regex.
### Back-references
* There are no back-references within this regex.
### Look-ahead and Look-behind
* This regex cotains neither look-ahead nor look-behind. 

## Author

I am learing a great deal about coding and am taking a shot a writing my first tutorial. If you'd like you can take a look at my github [ericy98](https://github.com/ericy98/)! Or email me any questions that may arise at ea.yarbrough98@gmail.com.
