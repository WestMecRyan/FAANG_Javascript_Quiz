# FAANG_Javascript_Quiz
An Advanced Javascript Quiz for fun!

## About Octals
In javascript numbers prefaced by a leading zero are converted into Octal.
Octal starts over after 7 so O17 is 15
Whereas 026 would be 22 because 2 x 8 is 16 + 6 is 22

In ECMA SCRIPT 6 you can use 0o prefix to declare an octal,
at which point 0o18 would throw an error because an 8 is not
a valid octal number but if you do 018 it will coerce it into
the decimal number 18

If you have to use a leading zero for some reason,
let's say you have a database of numbers that have leading zeros
you can pass do 
```
parseInt(dataBaseItem.toString(), 10);

## typeof typeof 1

Typeof is read right to left 
typeof returns a string of the type the item is

## sorting number array
Javascript allows dynamic arrays like
let someMixArr = ["1", true, 55, 1.42, "foo", {}];

If you want to sort this array all the characters have 
to be turned into strings first.
ascii for '[' is 91, ascii for 'Z' is 90, ascii for 'a' is 97
let someFunArr = [{}, 'a', 'z']

## checking loose equality, false, '0'

loose equality defaults to turning strings that contain a number
into strings if the equality check contained a number and it 
defaults to turning booleans into 0 and 1

`console.log(false == 'false');` //evaluates to false`
`console.log(false == '0'); //evaluates to true`


## Dealing with Floating Point numbers
`console.log(0.1+0.2)`
let sum = 0.1 + 0.2
sum.toFixed(2); // returns a string
// to get the string back to a number use
let roundedSum = Number(sum.toFixed(2));

## increasing the length of an array in javascript is possible
it just puts empty item slots in the array which return undefined
`let arr = [1,2,3]`
arr[6] = 9;
arr[5] // returns undefined

in Java arr[6] would be out of bounds you have to declare the length
of the array at time of creation.

// empty items can only be created when you create an array with
some length but don't populate the slots.
let newArr = new Array(5);

# stopping at 12 minute mark
