
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

( Sadly no uppercase support :( )

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
* [GUI](#GUI)
* [Syntax](#Syntax)
* [Datatypes](#Datatypes)
* [Screenmodes](#Screenmodes)
* [Variables](#Variables)
* [I/O](#Input-and-Output)
* [Loops](#Loops)
* [Ifnum](#Ifnum)
* [Functions](#Functions)
* [Filesystem](#Filesystem)
* [Pen](#Pen)
* [Music](#Music)
* [Other](#Other)


### GUI
Let's take a closer look at the GUI of the Project!  
  
Here's how it looks when you first start the Project:  
![IMG1](https://i.ibb.co/JdSFSvD/Download-3.png)  
You will probably notice a few a things: 
* The numbers on the left.  
They are here for telling you the number of line you are on.  
* Differently coloured text.  
Its for the different Datatypes and for potential errors you made.  
* The Black Box.  
That's your cursor!  
* The 3 Buttons!  
Those are the main control Buttons!  
Let's take a closer look!  

#### The Menu Button
That's the first Button. (from the left)  
It will allow you to go to the Menu and Back.  
Wondering how the Menu looks?  
Here is an Image:  
![MENU1](https://i.ibb.co/SXK37kg/Download-4.png)  
 Cool, right?
Left, there is the Keybind Mapper. There you can map special keys to do certain actions like Backspace or Autocompletion.  
Right, is the main part:  
We have Options like:  
* clear code - Clearing your current code.  
* examples - Shows a list of examples, you can load.  
* Autocomplete Highlighter - Toggles the highlighting of words that it want to autocorrect.  
* Save Code - Saving Code  
* Load Code - Loading Code. 
That's all ya gotta know :p  
  
#### The Import Image Button
Here you can import your Images with an Image Code you got from ( https://scratch.mit.edu/projects/392443979/ )  
Note: It will REPLACE your current line of code!  

  
  
#### The run Button
With this Button, you can run your Program.  
When it stops, you can just press the green Flag, to go back to the Editor.  


  
  

### Syntax
Here is the simple Command-Syntax:  
```
Command [arg1] [arg2] [arg3] [arg4] [arg5] [arg6]
```
[arg] is an Argument.  
There can be up to 6 Arguments per Command.  
We will now look at the things the Arguments can be. (Datatypes)  
  
  
### Datatypes
Let's look at all of the Datatypes you can use as Arguments!  
These are the 6 main Datatypes:  
  
**Values** `They can be a word or a number or a Variable. (variables can be used in places of values like this: $varname )`  
**Strings** `up to infinite values inside of a "" (like "test 1 2 3 lol")`  
**Operators** `can be "+, -, *, /, >, <, =, ≠, mode (depending on the Command)`  
**Operations** `can be round, amount, round_down, round_up, root, sin, cos, tan, asin, acos, atan, ln, log, e_ttpo, 10_ttpo, (ttpo: to the power of)`  
**comments** `up to 12 values or so. (mainly for commenting)`  
  
  
### Variables

Let's start with some basic Variables.  
  
To set a Variable to a value (and initialise it), use set and sets. 
(sets is basically set Variable to a String)  
```
set Test 100
sets Test2 "Test lul"
set Test $Test2
```
To do math, use math or 2math.  
```
math $var1 * $var2 var3
-set the output of var1 * var2 to var3.

2math sin $var1 var2
-set the ouput of sin of var1 to var2.
```

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

  
  
   
### Ifnum
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

  
  
  
  
### Filesystem
Low Level Commands are for manipulating Cells or/and the Pointer directly.  


  
  
  
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
cls
nl
+line 1 "hello, world!"
wait 5
 ``` 
 

