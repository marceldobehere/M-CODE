
## Table of contents
* [Description and Links](#M-CODE)
* [Features](#Features)
* [Commands and Syntax](#Commands)
* [Examples](#Examples)

# M-CODE
A new programming IDE and language on Scratch (by me)  
Here is some Documentation of my Programming IDE + language on Scratch.  
  
## Features
Here are some Features it has:  

* an Editor with automatic X/Y Scrolling
* Text/Image out
* colorcoded text (in the editor)
* Autocompletion
* Automatic error finding and marking
* a Cursor for easy typing and use with an Insert function 
* a Backspace function
* Mappable keys (for different keyboards)!
* Pen Support
* Text Support
* Math Support
* Variables Support
* Music Support
* Images
* a Filesystem
* I/O
* Randomisation
* Functions, loops and Ifnum

## Links
#### Here is the Project:
```
https://scratch.mit.edu/projects/387534263/
```

#### Here is the Main Forum Page:  
```
https://scratch.mit.edu/discuss/topic/397646/
```
#### Here is the Project to import Images:  
```
https://scratch.mit.edu/projects/392443979/
```

## Commands
#### Here is the full Command list:
```
https://scratch.mit.edu/discuss/topic/397643/
```
#### Lets go over the basics
* [Variables](#Variables)
* [Lists](#Lists)
* [I/O](#Input-and-Output)
* [Loops](#Loops)
* [Do if](#Do-if)
* [Functions](#Functions)
* [Low Level stuff](#Low-Level-Commands)
* [Other](#Other)




### Variables

Let's start with some basic Variables.  
  
To set up a Variable for later use, just use int.  

```
int Test
```
To set a Variable to a value, use set.  
```
set Test 100
```
To set a Variable to another Variable, use copy.  
```
copy Test Test2
```
To do Math with two Variables, use math.  
Note: The output will get set to the first Variable.  
```
( Supported Operations are Addition(+) Subtraction(-) Multiplication(*) Floor Division(/) )  
math Test * Test2
```
  
  
   
### Lists
Next up are Lists.  
  
To set up a List for later use, just use lint.  

```
lint Test (amount of elements)
```
To set an Element to a value, use lset.  
```
lset Test 1 5
```
This sets the first Element of the List to 5.  
  
To set an Element to a Variable, use vlset.  
```
vlset Test 1 var
```
This sets the first Element of the List to (var).  
  
   
Now we want to set the X'th Element of a List to a Variable.  
Just use vvlset.  
```
vvlset Test var1 var2
```
This sets the (var1) Element of the List to (var2).  
  
   
Now we want to set a Variable to some Element of a List!  
Just use lsetvar.  
```
lsetvar Test 1 var
```
This sets var to the first Element of the List .  
  
  
And now again with the X'th Element.  
Can you guess it?  
Its lsetvvar.  
```
lsetvvar Test var1 var2
```
This sets var2 to the (var2) Element of the List.  
  

   
   
### Input and Output
We have a few ways of Input and Output with S-CODE.  
#### Input
For input, we have input.
```
input var
```
This will prompt input and set var to the ASCII value of the input

#### Output
For Output we have a few Options:  
output.
```
ouput A
```
This will output A.  
  
  
output#.
```
ouput# 10
```
This will output 10 (a new line)  
  
  
For new lines we can also just use nl.
```
nl
```
  
  
Do you want to display Long Text?  
No Problemo! Just use phrase.
```
phrase Hello, World!
```
Can you guess what it will do?  
  
  
Now let's output a Variable!  
```
outvar var
```
This will output the Variable var. (Just like ouput# but with a Variable)  
  
  
Many People faced the HORROR of displaying the Value of a variable in Decimal.  
But with S-CODE it's as simple as outvardec.
```
outvardec var
```
This will output the decimal value of the Variable var.   
   
   
   
### Loops
Now let's get to the Loops!  
  
   
Loops look like this:  
```
loop var1 (= > < ≠) var2
...
if var1 (= > < ≠) var2 loop
```
the *loop* command starts a loop when a condition is given. (Like var1 > var2)  
Every Loop has to have 1 *if ...* command at the end of it where it will loop if a condition is met (Like var1 ≠ var2)  
Note: Loops, if and Do commands only work with variables (for now) so set a variable beforehand!  

  
  
   
### Do if
The Do if command works like the loop command but only once (no looping)
```
do if var1 (= > < ≠) var 2
...
stopdo
```
you can guess what how it works by now...  

  
  
   
### Functions
Functions are like Do if but without the if.  
Add them with this code:
```
function name
...
endfunc
```
Call a function with func.  
```
func test
```
Note: Functions use global variables like everything else and functions CANNOT have other Functions inside!!! (it could cause an endless loop of compiling)  

  
  
  
  
### Low Level Commands
Low Level Commands are for manipulating Cells or/and the Pointer directly.  
We have raw.  
This allows you to paste your own BF Code inside of the S-CODE.  
```
raw >>>+>-[>+<-]
```
Note: When using the raw command, you should always use goto beforehand AND the pointer HAS TO BE EXACTLY WHERE IT WAS BEFORE THE RAW CODE!!!!  
  
  
Then we have cellcopy.  
This allows you to copy one Cell to another.  
```
cellcopy 20 35
```
This copies the Cell 20 to the Cell 35.  
    
  
Then celllchange.  
It changes a cell by some amount
```
( You can only use + or - )
celllchange 10 + 2
```
This changed the Cell 10 by 2.   



And last but not least vcellchange.  
```
vcellchange 10 + var
```
This changed the Cell 10 by (var).  
  
  
And of Course goto.  
```
goto 10
```
It sets the Pointer to 10.  
  
  
   
### Other
Here are some Commands that don't fit in the other Categories:

#.  
```
# Your Comment goes here
 ``` 
It's for commenting.  
   

## Examples

Here are some Example Programs I made for you!  




### Hello, World!
 ``` 
phrase Hello, World!
 ``` 
 
 ### Number Comparator
 ``` 
int a
int b
phrase input number one: 
input a
outvar a
nl
phrase input number two: 
input b
outvar b

loop a = b
nl
outvar a
phrase =
outvar b
if a = b loop

loop a > b
nl
outvar a
phrase >
outvar b
if a > b loop

loop a < b
nl
outvar a
phrase <
outvar b
if a < b loop
 ```  
 ### get decimal ASCII of input
 ``` 
int a
phrase Enter a character
loop a = a
input a
nl
outvar a
phrase : 
outvardec a
if a = a loop
 ``` 
