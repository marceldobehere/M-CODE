
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
* [Logic](#Logic)
* [I/O](#Input-and-Output)
* [Loops](#Loops)
* [Ifnum](#Ifnum)
* [Functions](#Functions)
* [Goto and Jump](#Goto-and-Jump)
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
  
**Values** `They can be a word or a number or a Variable. (variables can be used in places of values like this: $varname ) - are coloured dark blue`    
**Strings** `up to infinite values inside of a "" (like "test 1 2 3 lol") - are coloured green`  
**Operators** `can be "+, -, *, /, >, <, =, ≠, mode (depending on the Command) - are coloured purple`  
(mode would be for the time like second, minute, hour, day, month, year)  
**Operations** `can be round, amount, round_down, round_up, root, sin, cos, tan, asin, acos, atan, ln, log, e_ttpo, 10_ttpo, (ttpo: to the power of) - are coloured light green` 
**comments** `up to 12 values or so. (mainly for commenting) - are coloured grey`  
  
  

### Screenmodes
Here are the 3 Screenmodes changed with the screenmode command.  
1 - Editor (maybe for programs involving changing the code mid-execution)  
2 - Text-out (for Displaying Text)  
3 - Draw-out (for Drawing, loading Images, or writing Text in some random places)  
  
Example:  
```
screenmode 2
```
  
### Variables
Here are the basics you need with Variables:  
  
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
-sets the output of (var1 * var2) to var3.

2math sin $var1 var2
-sets the ouput of (sin of var1) to var2.
```
Then we also have more commands about Variables:  
```
ran 1 10 var1
-sets var1 to random value (rounded) between 1 and 10.

join hello $test var1
-joins hello and the variable test into the Variable var1

letter 1 $text var1
-sets var1 to the first letter of the Variable text

sletter 1 "hello this is a test" var1
-sets var1 to the first letter of "hello this is a test" (would be h)

lenght hoiiii123 var1
-sets var1 to the lenght of hoiiii123

contains? $text aa var1
-sets var1 to true/false, depending on if the variable text has aa inside of it.

scontains? "test aaaaaa lol" aa var1
-sets var1 to true/false, depending on if "test aaaaaa lol" has aa inside of it.

```

### Logic
We also have logic in form of bitwise Operations.  
We use the command op_[and, or, not] like this:  
```
op_and $var1 $var2 var3
-sets var3 to true/false depending on if var1 and var2 are equal to one.
```
  
  
  
### Input and Output
We have a few ways of Input and Output.  
#### Input
For input, we have ask and vask.
```
ask "hello! how are you?" var1
-asks "hello! how are you?" and sets the awnser to var1

vask hello var1
-asks hello and sets the awnser to var1
```
of course there are other inputs like:  
```
time minute var1
-sets the current minute to var1

m_x var1
-sets var 1 to the Mouse X Position.

m_y var1
-sets var 1 to the Mouse Y Position.

m_x var1
-sets var1 to true/false, depending on if the Left Mouse Button is clicked.

key a var1
-sets var1 to true/false, depending on if the key a is pressed.
```



#### Output
For Output we have some Commands: 

* nl
```
nl
```
This will add a new Line to the output.  
  
* cls
```
cls
```
This will delete every line.  
  
* +line
```
+line 1 "test"
```
This will add test to line 1.  
  
* +vline
```
+line 1 12
```
This will add 12 to line 1.  
  
* delline
```
delline 2
```
This deletes the line 2.  
  
   
   
### Loops
Loops look like this:  
```
:loop 10
...
end
```
This code will loop ... 10 times before continuing.
  
  
   
### Ifnum
The Ifnum Command skips the next few lines if a condition ISN'T met.  
```
set var1 0
set var2 5
vask Number: var1
ifnum $var1 = $var2 2
+line 1 "yay the number is 5!"
endall

+line 1 "awww. the number is not "
+vline 1 $var1
+line 1 "."
endall

``` 
  
   
### Functions
Functions are pretty simple.  
Add them with this code: 
```
:func "function lol"
...
end


func "function lol"

```
Note: Functions get skipped when "initialising them" and only get executed when called.  
Note: When calling a function, you can add up to 3 extra values to be inside the function like "func "test" 154 20 $var1" and their name is this:  
```
func_(function name)_[1,2,3]
like this: +vline 1 $func_test_1

(Note: it won't work on functions with spaces in the name...)
```
  
  
  
  
### Goto and Jump
First, lets look at goto.  

```
:goto "test goto"
(sets up a jump point no "end" required and therefore won't get skipped when running)
...



goto "test goto"
(jumps to the point)
```
Now, let's look at jump.  
jump is pretty easy, since it just jumps to a specific line number.  
Note: The line should be empty so there won't be any errors...  
```
jump 10
```





### Filesystem
basically you can create, delete and load files with some commands.  

```
new_file "test" .txt
-makes a new file called "test" with the extension .txt

sets_file "test.txt" "lol"
-sets the content of text.txt to "lol"

setv_file "test.txt" $lol
-sets the content of text.txt to the variable lol

nlto_file "test.txt"
-adds a new line to a file

addtos_file / addtov_file
-like (sets/setv)_file but just adding the data

data_line_file "test.txt" 1 var1
-sets var1 to the first line of the data in test.txt

#datav_line_file "test.txt" lol var1
-sets var1 to the element number of "lol" in test.txt (lol has to be the whole element!)

#datas_line_file "test.txt" "test lol" var1
-sets var1 to the element number of "test lol" in test.txt (lol has to be the whole element!)

delline_file "test.txt" 2
-deletes the second line of file test.txt

del_file "test.txt"
-deletes the file

run_file "test.txt"
-runs the file (could lead to lag and acts like a goto)

```
  
  
### Pen
a
  
  
### Music
a
  
  

  
  
  
### Other
Here are some Commands that don't fit in the other Categories:

#.  
```
# Your Comment goes here
 ``` 
It's for commenting.  
   
endall.  
```
endall
 ``` 
Stops the program completely.  

## Examples

Here are some Example Programs I made for you!  




### Hello, World!
 ``` 
cls
nl
+line 1 "hello, world!"
wait 5
 ``` 
 

