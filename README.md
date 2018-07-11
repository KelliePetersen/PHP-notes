# PHP Basics

## Contents

- [Important Notes](#important-notes)  
- [Basics](#basics)  
- [Strings](#strings)  
  - [Length and White Space](#length-and-white-space)  
  - [Character Types](#character-types)  
- [Arrays](#arrays)  
- [Conditional Statements and Loops](#conditional-statements-and-loops)  
- [Functions](#functions)  
- [Classes](#classes)  
- [Objects](#objects)  
- [Iterators and Generators](#iterators-and-generators)

## Important Notes
PHP is saved in .php files and can be used in .html files. It must be enclosed in PHP opening and closing tags.  
`<?php //write your PHP here ?>`

## Basics

| Description | PHP |
| --- | --- |
| Single-line Comment | // I am a comment or # I am a comment |
| Multi-line Comment| /* I am a multi-line comment \*/ |
| Defining variables | $myVariable = "I am a variable"; |
| Printing lines (1 value only) | print("Hello $name"); or print "Hello $name"; |
| Printing lines (multiple values) | echo "Hello $name"; |
| Swap values | [$a, $b] = [$b, $a]; |

## Strings

### Length and White Space

### Character Types  

| Description | PHP |
| --- | --- |
| Check if all characters are lowercase | ctype_lower($string) |
| Check if all characters are uppercase | ctype_upper($string) |
| Check if all characters are letters | ctype_alpha($string) |
| Check if all characters are alphanumeric | ctype_alnum($string) |
| Check if all characters are digits | ctype_digit($string) |
| Check if all characters are decimal | is_float($string) |
| Check if all characters are numeric | is_numeric($string) |
| Check if all characters are space | ctype_space($string) |
| Check if all characters are printable | ctype_print($string) |
| Checks if characters are control characters | ctype_cntrl($string) |

## Arrays  

## Conditional Statements and Loops
PHP has two different ways to enclose conditional statements and loops: brackets and colons.  
`while (condition) { ... }` and `while (condition) : ... endwhile;`  

### While Loop
```
while ($i < 10) {
  // do a thing
}
```
```
while ($i < 10):
  // do a thing
endwhile;
```
```
do {
  // do a thing
}
while ($i < 10);
```

### if/else
You can use "else if" or "elseif". 
```
if ($i < 10) {
  // do a thing
} else if ($i === 5) {
  // do another thing
} else {
  // whatever
}
```
If using colons instead of brackets, you *must* use "elseif".
```
if ($i < 10):
  // do a thing
elseif ($i === 5):
  // do another thing
else:
  // whatever
endif;
```

### Ternary Operator
Structure: `$var = (condition ? trueResult : falseResult);`  
Example: `$greeting = ($time < 12 ? "Good morning!" : "Good afternoon.");`  

### Switch
```
switch(expression) {
  case value1:
    // do a thing
    break;
  case value2:
    // do a different thing
    break;
  default:
    // do the default thing
} 
```

### For Loops
```
for (let $i = 0; $i < 10; $i++) { 
  // do a thing
}
```
```
for (let $i = 0; $i < 10; $i++):
  // do a thing
endfor;
```
Loops for indexed arrays:
```
foreach ($array as $value) {
  // do a thing
}
```
```
foreach ($array as $value) :
  // do a thing
endforeach;
```
Loops for associative arrays:
```
foreach ($array as $key => $value) { 
  // do a thing
}
```

## Functions

## Classes

## Objects

## Iterators and Generators
