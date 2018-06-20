```
+------------------------------------+  
|                                    |  
|                                    |  
|    \                /              |  
|     \              /               |  
|      \            /   o            |  
|       \          /                 |  
|        \        /     |            |  
|         \      /      |            |  
|          \    /       |            |  
|           \  /        |            |  
|            \/        _-_           |  
|                                    |  
|            Essentials              |  
|                                    |  
|                                    |  
|                                    |  
|                                    |  
|                                    |  
|       Weathered Paperweight        |  
|                                    |  
|                                    |  
|                                    |  
|                                    |  
+------------------------------------+  
```
---  

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<a rel="license"
href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img
alt="Creative Commons Licence" style="border-width:0"
src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png"
/></a><br /><span xmlns:dct="http://purl.org/dc/terms/"
href="http://purl.org/dc/dcmitype/Text" property="dct:title"
rel="dct:type">Vi Essentials</span> by <span
xmlns:cc="http://creativecommons.org/ns#"
property="cc:attributionName">Weathered Paperweight</span>
is licensed under a <a rel="license"
href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative
Commons Attribution-NonCommercial-NoDerivatives 4.0
International License</a>.
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>  

---------


Table of contents
=================

1. Introduction
   1. The importance of vi
   2. What all this book covers
   3. Who should read this book
   4. Who should avoid this book
   5. How to read this book
      * Prerequisite
   6. Feedback is important 
   7. Colophon
2. Vi Editor
   1. Modes in vi
      * Normal Mode
      * Insert Mode
      * ex mode
   2. Let's get started
      * Some Notes
3. Basic Movements
   1. The movement commands
   2. Move by characters
      * Alternatives to hjkl
      * Move by lines
      * Move by Words
   3. Using a count
   4. Summary 
4. Basic Editing
   1. Insert Mode
   2. Ex Mode
   3. Operator Commands
      * Change Operator
      * Delete Operator
      * Yank Operator
      * Put Operator
   4. Operator with count
   5. Whole Line Editing
   6. Summary


#### Chapter 1 
---------------
Introduction
======================
Working with text is pretty common in Computer Systems. All
programs are written in plain text, many
configuration files are written in plain text. Also for
quick notes, plain text is far more quick and useful than
processed documents. Until and unless a document needs to be
presented in a well formatted way, we do not need heavy
processing of text. Also, it should be noted that, before
presentation of any information (in formats like Word Document, PDF,
Powerpoint Presentation etc.), user needs to
collect and store the information first in plain text, then only he
or she will be able to present it in desired format.

The usefulness of text editing led the way to have a text 
editor present in any OS. Like, Windows provides
Notepad.exe, Mac OS provides TextEdit, any version of 
Gnome based Linux provides GEdit and almost all the
\*nix systems by default provide vi editor or Vim (vi
improved) for editing text.

1.1 The importance of vi
------------------------
While there are many text editors available (Both GUI Based
and Text Based), vi is pretty popular in \*nix community.
Reasons behind this are following -  
 1. vi editor is standardized by POSIX, so any POSIX compliant
    system must have this editor. Thus it can be life saver
    at times when you have to perform some text editing but you
    do not have any other option available to you.
 2. Also if you are connecting to other machine using ssh,
    no GUI based editor will work. So, vi can be used to
    edit files in remote systems as and when required.
 3. vi is extremely fast and runs on low resources.
 4. While using vi editor users need not use mouse and there
    are very few control key combination required in vi.
    This saves a lot of time.
 5. As vi is available everywhere and many Unix/Linux users use this
    text editor, you can get plenty of help over the internet.
    So, day to day job becomes easier.  

Due to the reasons mentioned above, many programmers and
system administrators rely on vi editor.

1.2 What all this book covers
-----------------------------
This book is mainly focused on the basic commands of vi
editor, which is available in any other improved version of
vi like vim, nvi, elvis etc. So, all the commands and
instructions available in the book will be applicable for
basic vi editor as well as any improved version of it.
This book does not contain any advanced feature which vim
or other feature-rich clone of vi editor provides. It leaves
the reader in a stage where he or she knows just enough for
basic text editing using vi. From there he or she can take 
it forward for performing complex editing tasks easily.

1.3 Who should read this book
-----------------------------
If you are thinking whether to read this book, please check
if you fall into either of the following categories -

 1. You just started using vi and are getting stuck at times
    and you need some help to get out of the situation.
 2. You had used vi editor previously but may be due to no
    use for long time you have forgotten many commands.
    In other words you need a quick refresher of vi editor.
 3. You are pretty enthusiastic about learning vi editor and
    as you read this book you are ready to open the terminal
    and actually edit some files to check how vi editor works.
 4. If you want to learn any vi editor clone (like nvi, vim
    and elvis). Though this book will not cover all details
    of a specific vi clone, it will be enough to grab the 
    basics and this book will leave you at a stage from where
    you can take it forward and learn any clone of vi.

1.4 Who should avoid this book
------------------------------
This book may dissatisfy you if - 
 1. You already know the basics of how to use vi editor
    or any of its clones.
 2. You are looking for a quick reference of all the vi
    commands.
 3. You want to learn vi editor and its usages by only 
    reading this book (and not doing anything in vi).

1.5 How to read this book
-------------------------
Open this book, in your favourite web browser and parallelly 
open vi editor in a terminal window or gvim (if you are 
running Windows). As you read through the chapters, you can 
experiment with the commands and instructions written in 
this book. Repeat the commands and practice until you are 
well familiar with the commands and it has become your second
nature to use them. Then move on to next chapter. Repeat the 
process until you have finished.
### 1.5.1 Prerequisite 
 1. Computer or tablet which has vi/vim/nvi/elvis editor
    installed. If you are on Windows and want to have
    vi, you can go for gvim. Google this phrase "gvim for
    windows".
 2. Reader should have knowledge on how to move between
    directories in command line and how to create
    directories using commands.
 3. Patience. It takes a lot of time to get familiar
    with all the controls of vi. But this actually pays 
    off in long run.

1.6 Feedback is important
-------------------------
This book is an ongoing project, if you find any mistake or
you have a suggestion please raise an issue here -
https://github.com/weathered-paperweight/vi/issues
Your changes and suggestions may get into future releases.

1.7 Colophon
-------------
This book is written using VIM - Vi Improved 7.4 on a
Lenovo G50-70 laptop running Linux Mint 18.1 Cinnamon 64
bit. All the movements and operators have been tested in vi,nvi, vile and
vim editor.



### Chapter 2
-------------
vi Editor
=========
In earlier days of Unix, only text editor available was
`ed`, which still today is available in any POSIX compliant
System but it is really painful to work with ed as it is a 
line based editor. That means, it displays one
line of text at a time on the command line and allows users to make
some change and save the line to file. Struggling with the lack of a 
good text editor in UNIX, the then student of *University of 
California at Berkeley*, Bill Joy developed `ex` text editor
which was a superset of `ed` text editor. Still it was
lacking one important thing, a *visual interface*. So, he started
developing a visual interface for ex editor around 1976.
Vi editor got its name from the fact that it is a *visual
interface* to the `ex` text editor. Such a gift can be 
expected from a co-founder of _Sun Microsystems_. In spite of
the fact that, GUI has gone a long way from where it was at
1976,`vi` is still a very popular choice as a text editor. 
It is not surprising that it has made its way into the
__POSIX Standards__. While vi editor might not be intuitive and
easy for beginners, a few days of practice can make users 
edit files a lot faster and in a convenient way.

2.1 Modes in vi
---------------
vi editor is a modal editor, which means that, depending on
the mode vi editor is, commands change their course of
action. While using vi editor you don't have to move your
hands from keyboard to mouse, which is why it makes 
editing faster. Most of the commands in vi editor resides
in the typing section of your keyboard, to facilitate this vi
comes with the concept of different modes. vi offers three
modes of operation. Following are details of them -

### 2.1.1 Normal Mode
This is the mode when vi editor first opens. This mode
facilitates moving around a file and run commands which
changes the text in the file.

### 2.1.2 Insert Mode
In this mode users can type in the keyboard and text gets
inserted into the file. This behavior is similar to the one
you can expect in a Graphical Editor like Notepad or GEdit.

### 2.1.3 ex mode
vi is an extension to the text editor `ex`, so it supports
commands from ex editor as well. This mode in vi allows
the users to run ex commands. At times ex commands are far
more convenient to use than using vi commands. Also to
configure the behavior of vi editor, user need ex mode.

In the beginning, it may be pretty difficult to understand
the concept of modes and it confuses all beginners. To add
to the difficulty, there are keys which changes the mode on
the fly, changes cursor positions. So, it is confusing at
first, but as you practice, this is easy to use.

2.2 Let's get started
---------------------
After reading until this point, it can be a fair estimate
that you want your hands to get dirty on the command line.
Now is the time to do some actual stuff. To perform the
operations in this section, I would suggest you to create a
directory of your choice and navigate into it. In the
subsequent hands-on sections also, you can use this directory.
First thing we'll run on command line is `vi` command and see how
the editor looks like.
```
+------------------------+
| $ mkdir vi-essentials  |
| $ cd vi-essentials/    |
| $ vi                   |
+------------------------+
```
Once you hit this command on the command prompt, depending
on the installation, you can either find a vim editor
window opened or a classic vi window opened. Following are the
two different editors' default looks -
```
+--------------------------------------------------------+ 
|~                                                       | 
|~                                                       |
|~                 VIM - Vi IMproved                     |
|~                                                       |
|~                  version 7.4.1689                     |
|~              by Bram Moolenaar et al.                 |
|Modified by pkg-vim-maintainers@lists.alioth.debian.or  |
|~    Vim is open source and freely distributable        |
|~                                                       |
|~           Become a registered Vim user!               |
|~   type  :help register<Enter>   for information       |
|~                                                       |
|~   type  :q<Enter>               to exit               |
|~   type  :help<Enter>  or  <F1>  for on-line help      |
|~   type  :help version7<Enter>   for version info      |
|~                                                       |
|~                                                       |
|~                                                       |
|                                    0,0-1         All   |
+--------------------------------------------------------+
              Vim editor with no file input
```

```
+--------------------------------------------------------+
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|/tmp/vi.FajNUg: new file: line 1                        |
+--------------------------------------------------------+ 
                      vi editor
```

In case you are using nvi, you can find the following
```
+--------------------------------------------------------+
|                                                        |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|~                                                       |
|/tmp/vi.WjfEDi: new file: line 1                        |
+--------------------------------------------------------+
                     nvi editor
```
Some points to be noticed here, first is that, once you are
in, you loose access to terminal, the second point to notice
is, you see screen full of '~' (tilde) character followed by 
blank lines (except for vim, which shows some information
instead).  
Also you see some information printed on the last line.

Now, we'll cover them one by one.
 1. When you open vi it replaces your terminal - you can get
    out of vi editor by hitting `<Esc>` key and typing `:q!`.
    The `<Esc>` key puts you in normal mode. While you type
    `:` in normal mode, mode changes to ex mode and  `q` is
    the command to exit out of the vi editor, `!` is
    added to it just in case you have made some changes in
    the buffer, it will overwrite the changes and allow you
    to get back to terminal without saving anything. We'll 
    talk about these later while editing actual files.
 2. The `~` denotes that these lines are not in file. So, if
    you see the whole screen full of tilde characters
    followed by blank lines, it means the file is empty. In
    case of vim editor, instead of showing blank lines,
    it shows some information on how to get out of vim or how 
    to get help in vim. But as soon as a character is entered,
    this information is hidden. None of these are part of your
    text content.
 3. The last line shows some information. Basically, it
    shows the position of the cursor in the file like, on
    which line cursor is or on which column the cursor is
    waiting etc. The other part of information shown in the
    last line is about the file you are writing; as vi
    editor is not opened for a particular file, it opens a
    buffer.
    
You can close the vi editor by typing `<Esc> :q!`

### 2.2.1 Some Notes
1. Vi always puts you in a buffer while opening. While
   opening vi, if it was not supplied a file name, it will
   open empty buffer and when you save the content, then only 
   it gets saved in a file with a name of your choice. In
   case of editing an existing file, vi opens a buffer with
   the content from the file and when you are ready to save,
   it actually saves the changed content in the file.
2. Vi is case-sensitive. So, `q` and `Q` are two different
   commands. So, if you are experiencing an unexpected
   output, please check the `<Caps Lock>` first.

Now it's time to practice it over and over again. Once you
are comfortable getting in and out of vi editor, you can move
forward with doing some actual change in the buffer and save
to file.

```
+------------------------------------------------------------+
| A note on presentation, this book is completely written in |
| plain text, the code and screen changes will be presented  |
| within an ASCII box like the way it is presented in this   | 
| section.                                                   |
+------------------------------------------------------------+
```


#### Chapter 3
---------------
Basic Movements
===============
Moving around the contents of a file is the most common
thing anyone does. Once you have opened a file and want to
change its contents, you must move cursor to exact location
and perform the change. Also, movement commands form the
basis of editing commands. So, they are pretty much used 
every time you open vi.
Vi editor provides a very easy and fast way to navigate
around the file content. Well to be frank, it is not that
easy at first but after some movements, it is pretty easy.
Because the movement commands reside at your right hand home
row, the easiest location to reach on the keyboard. 

3.1 The movement commands
-------------------------
To use the movement commands, you will need to have a file
which has some text in it. So, you can copy an existing file
full of text to your working directory and try using the 
movement commands on it.
```
+----------------------------------------------------------+
|$ vi ~/vi-essentials/book                                 |
+----------------------------------------------------------+
```
### 3.1.1 Move by characters
While you have opened the file in vi editor, the 
cursor resides at the first character of the file. 
Press `<Esc>` key once just to make sure, you are in
normal mode.
In normal mode you can use the movement commands 
and move the cursor to your desired position.

Following are the commands to move cursor in  Normal
Mode -  
h - move cursor to the left  
j - move cursor one line down  
k - move cursor one line up  
l - move cursor to the right  

Pretty confusing (who assigns 'l' to move right), but
you should notice that all the commands are there on
your right hand home row. After some movements, this 
would be fine and it will make the most sense.

Following guide may be of use -  
h - resides on left  
j - has hook down  
k - points up  
l - is on right  

Or may be you can put a sticker on your desktop monitor
with the following print out -
```
                        k
                        ^ 
                     h<   >l
                        v 
                        j
```
Practice this movement until you don't have to think 
which key to use for which direction.

###  3.1.2 Alternatives to hjkl
All the hassles can be minimized and all confusions
can be eliminated by just using the arrow keys in
your keyboard. But think this way, it will slow you
down while editing text and it can distract you to
search for arrow keys in your keyboard while in
between a serious editing. Choice is yours but
recommendation would be to use hjkl.
Another alternative to `h` and `l` is to use
`<Backspace>` and `<Space>`. While it is true that
`<Space>` key is also easy to reach, `<Backspace>` is
not. Also, you do not get the flexibility to move
line up or down with this combination.

### 3.1.3 Move by lines
Once you are comfortable moving by characters, now
it's time to move in the line and out of the line. 
The following line level movements can be performed
in vi editor normal mode -  
```
0 - move to the first character of the line
$ - move to the end of the line
^ - move to the first non-blank character of line
+ - move to first non-blank character of the next line  
<Enter> - move to first non-blank character of the next 
    line
- - move to first non-blank character of the previous 
    line
```
### 3.1.4 Move by Words
With the commands covered till now, you should be pretty 
much comfortable in moving around a file. Still something 
is missing. Perhaps, you also felt that, it would be nice 
to tap into the middle of a line or move to a particular
word and change it.
To do so, there are commands to move back and forth 
between words in vi editor.
These are the three basic word movement commands to be
used in normal mode -  
```
w - cursor moves to the first character of the next word  
e - cursor moves to the last character of the  
    current/next word. If the cursor is in the last  
    character of the current word, it moves to the  
    last of the next word. Otherwise, it moves to the  
    last character of the current word  
b - cursor moves to the first character of the  
    previous/current word. If the cursor is in the  
    first character of a word, then it moves to the  
    first character of the previous word. Otherwise,  
    it moves to the first character of the current  
    word.  
```
You might have noticed that while moving, special
characters/punctuations are also treated as a single
word, so 'vi.' is actually two different words. But at
times, you may want to treat them a single word. To
do so, you just have to use capital letters of the 
command (W, E, B). Just try it out, you will understand
the difference.

Let's have a quick hands-on of these movement commands. To
do this, open vi editor with a file full of text or download
this one and open in vi-
https://github.com/weathered-paperweight/vi-essentials/blob/master/data.txt

Move to the directory you have downloaded the file and open
using vi -  
```
+-------------------------------------------------------+
|$ vi data.txt                                          |
+-------------------------------------------------------+
```
This will open the file with the content of the file-  
```
+-----------------------------------------------------------+
|In its simplest form, Data is a collection of information. |
|This information may be of any type, numbers, words,       |
|observations, measurement or even just a description.      |
|                                                           |
|With that said, let’s dive deeper. Data can be of two      |
|forms,                                                     |
|    Qualitative – it represents description or quality of  |
|                  something. Analogous to Adjectives in    |
|                  grammars.                                |
|    Quantitative – it represents numerical information     |
|                   like 8 chairs, 9.8 meters, 20 litters   |
|                   etc.                                    |
|                                                           |
|Now, in a way, we can divide quantitative data into two    |
|parts as well,                                             |
|    Discrete – it has some restrictions on it. It can      |
|               take certain values and the values are      |
|               distinct and separate. This data can’t      | 
|		be broken in smaller units.                 |
|               It’s typically counted in whole numbers.    |
|               For example: number of pages in a book,     |
|               gender of a person (male or female),        |
|		blood group of a person (A, B, O, AB) etc.  |
|    Continuous – it is the data that can be measured and   |
|                 broken down in smaller parts and still    | 
|		  be meaningful. It is the data that can be |
|		  measured on a scale and can have any      |
|		  value                                     |
|		  within a range.                           |
|                 For example: height of a person, length   |
|                 of a road, volume of a cube etc.          |
+-----------------------------------------------------------+
```
When you first open vi, the cursor resides below the first
character of the file. In this case, it resides below the
first **I** in the file.
At this point, we'll go through the movement commands
(`h`,`j`,`k`,`l`).
First we'll try hitting `h`. As there is nothing on the left
of the character, cursor won't move anywhere.
So, now we'll try the next one which is `j`. This will bring
the cursor down one line on the second line on the first
character, that is **T**. Now we'll try hitting `k` which
will again bring back the cursor on the first line first
character, which is **I**. In short, this will bring you
back to the initial position. Now, we'll try the last one,
`l`, this will bring the cursor to the right below the
character **n**. From here, you can try hitting `h` which
will again bring you back to the initial position. Try using
these commands for a fair amount of time, until your brain
gets accustomed to it and you can automatically navigate the
cursor without thinking.  
In case, you have accidentally hit on some key which puts
you in _Insert Mode_, immediately hit `<Esc>` key or 
`<Ctrl> + [` combination to change the mode back to _Normal Mode_.  

Once you are accustomed to the basic movements, try the
other movement commands, like `0`, `$`, `+`, `<Enter>`, `^`,
`-`, `w`, `e`, `b`, `B`, `E`, `W`. Try to understand them by
using them on a real text file. It will be automatic after
sometime.  

3.2 Using a count
-----------------
While it is possible to traverse the whole file with these
simple commands only but you can actually make the movements
extremely fast by simply putting a count in front of the
motion command. For example, if you want to move 9 lines below,
you can press `j` 9 times or you can use `9j`, the cursor
will immediately move 9 lines below. Similarly, if you need
to move 9 lines up, you can use `9k`. The same goes with other
movement commands as well. So, `2h`, `3l`, `5k`, `6w`, `6W`,
`6B`, `7b`, `8e`, `9E`, `4$`, `9+`, `8-` are also valid movements.
The  movement commands that do not work with a count is `0`
and `^`.
Also, the `$` command works with counts a bit differently. If
you press `4$`, it will move to the last of 3 lines below.
Actually, the first `$` is used to move to the
last of the current line. Then, it applies the other 3 `$`
commands to move three lines below to the end of the line.

3.3 Summary 
-----------
In this chapter we learnt a lot about moving around the file
content. So, it is better to jot them down and make a table
for future reference.
```
+===================================================+
|              Summary of  Movements                |
|===================================================|
|Movement                              |  Commands  |
|--------------------------------------|------------|
|left arrow, down arrow, up arrow,     |  h, j, k, l|
|right arrow                           |            |
|--------------------------------------|------------|
|To first non-blank character of       |  ^         | 
|current line                          |            |
|--------------------------------------|------------|
|To first non-blank character of next  |  + or      |   
|line                                  |  <Enter>   |
|--------------------------------------|------------|
|To first non-blank character of       |  -         | 
|previous line                         |            |
|--------------------------------------|------------|
|To end of word                        |  e or E    |
|--------------------------------------|------------|
|Forward by word                       |  w or W    |
|--------------------------------------|------------|
|Backward by word                      |  b or B    |
|--------------------------------------|------------|
|To end of line                        |  $         |
|--------------------------------------|------------|
|To beginning of line                  |  0         | 
|--------------------------------------|------------|
|Move 5 characters left                |  5h        |
|--------------------------------------|------------|
|Move 5 characters right               |  5l        |
|--------------------------------------|------------|
|Move 5 lines up                       |  5k        |
|--------------------------------------|------------|
|Move 5 lines below                    |  5j        |
|--------------------------------------|------------|
|Move 5 words forward to the first     |  5w        |
|--------------------------------------|------------|
|Move to the first of 5 words          |  5W        |
|forward not counting  Punctuations    |            |
|--------------------------------------|------------|
|Move 6 words forward to the last      |  6e        |
|--------------------------------------|------------|
|Move 7 words forward to the last not  |  6E        |
|counting punctuation                  |            |
|--------------------------------------|------------|
|Move 3 words backward to the first    |  3b        |
|--------------------------------------|------------|
|Move 4 words backward to the first    |  4B        |
|not counting punctuation              |            |
|--------------------------------------|------------| 
|Move to the last of 3 lines below     |  4$        |
|--------------------------------------|------------|
|Move to the start of 5 lines above    |  5-        |
|--------------------------------------|------------|
|Move to the start of 6 lines below    |  6+        |
+--------------------------------------|------------+
```
These are pretty much all the basic movement commands, using
which you can move through a file. We'll look at other tools
for movement. But you should be pretty much comfortable with
the current set of movement commands before moving further.
As mentioned earlier, these form the basis of editing commands.
In the next chapter, we'll look into the basic editing 
commands which work in conjunction with these movement commands.


### Chapter 4 
-------------

Basic Editing
================
Till now we have seen how to move by characters, words and
lines, go to start and end of a line, go to start of
previous, current and next lines. These consist the basic
movements.  
Now it's time to understand basics of some editing. In this
chapter we'll look into some commands which are used
for editing text. Some command may put you into 
_Insert Mode_, so be careful on what you are doing and 
if you are in confusion about the mode, press `<Esc>` key
or `Ctrl+[` (Press and hold `<Ctrl>` key and press `[` key).
This will put you back into _Normal mode_.

4.1 Insert Mode
---------------
Till this point whatever commands we have used, we used them
in normal mode. That means, whatever we have done, we did
not make any change to the actual content of the file.
We never changed the mode of vi to Insert mode or used any
command which changes any text, even if we did, we
always used `<Esc> :q!` to get out of vi, which assures that
the file you opened in vi, is left intact.  But now, we are
going to make changes to the content of the file. We have to
use Insert mode to do so.  
In Insert mode, your key hits are used as an input to file 
content and it gets stored into the buffer until you either
save or discard the changes. There are many commands to be 
used in Normal Mode to change the mode to Insert Mode. Your
key hits will be treated as an input to the file content
when you are in Insert Mode. As you read through this chapter
and the next one, you will discover them one by one.  

The first command that changes the mode of vi editor is `i`.
In Normal mode, if you press `i`, it will enter Insert
mode and whatever key you press will be treated as an input
to the buffer content and you will see the change immediately.
Let's start with an empty file, we'll add some content in
it and save it.  
```
+---------------------------------------------------------+
|$ cd ~/vi-essentials/                                    |
|$ vi                                                     |
+---------------------------------------------------------+
```
This will open the vi editor like we've seen earlier. Now
hit `i`. The editor will enter the Insert mode. Some clones
of vi will show the mode information on the last line of the
screen.  
If you press any key, they will be added to the screen in
front and will be getting stored in the buffer. It is very
common to have mode confusion at this point. If your editor
shows the mode in the last line of the screen, you are
saved. Otherwise, it is difficult understand. If you are not
seeing as you are typing, then please press `<Esc>` key or
`Ctrl+[` key combination and again hit `i` key. This will
put you in Insert Mode. Keep typing your heart's content in
it and once you are happy, go back to Normal mode by pressing
`<Esc>` or `Ctrl+[`. Make it a habit to return to Normal
Mode as soon as your typing is over.**It is always better to
leave `vi` in _Normal Mode_ when you are not typing**. If you 
forget to return to _Normal Mode_ and want to move cursor 
using movement commands, they will be taken as input to the
file content. So, make it a habit from day one to return to
_Normal Mode_ as soon as you are done with typing.   

Once you are done with typing, you have many choices. You can save the
content to a file, you can discard the content and exit or 
you can make the whole screen empty again and start fresh.
To do any of these you have to enter `ex` mode.

4.2 Ex Mode
-----------
When you are in _Normal Mode_, you simply type `:` and it
moves to ex mode and you can see cursor waiting for you in
the bottom left corner of your screen after a `:`. Now type a 
command and hit `<Enter>` key and the command gets executed.  

There are many commands you can use in ex mode but for our
current purpose, we can use either of the following -
```
+-----------------------------------------------------------+
|  Command      |   Action                                  |
|---------------|-------------------------------------------|
|:w [file name] | This is Save Command. A new file is       |
|               | created with name 'file name' and the     |
|               | buffer content is saved in the file.      |
|               | If the file exists, it won't allow        |
|               | you to save.                              |
|---------------|-------------------------------------------|
|:w! [file name]| If the file exists with name 'file name', |
|               | the file is overwritten with the content  |
|               | otherwise, a new file is created. Please  |
|               | be careful while using this command. Im-  |
|               | proper use of this can loss existing data |
|---------------|-------------------------------------------|
|:q             | This is Quit command. So, it will try to  |
|               | quit the editor. But will show an error   |
|               | mentioning that the  content of the       |
|               | buffer is not saved                       |
|---------------|-------------------------------------------|
|:wq            | Combined Save and Quit Command. So, it    |
|               | will try to save the content but as no    |
|               | file name is mentioned, it cannot save    |
|               | the buffer content and will show similar  |
|               | error as before                           |
|---------------|-------------------------------------------|
|:wq [file name]| Combined Save and Quit Command. So, the   |
|               | content will be saved to file named 'file |
|               | name' and quit the editor.                |
|---------------|-------------------------------------------|
|:e!            | This command is issued to discard the     |
|               | changes. As we started with empty file,   | 
|               | a blank screen will be shown discarding   |
|               | all the changes.                          |
|---------------|-------------------------------------------|
|:q!            | Will discard the changes and exit vi      |
+-----------------------------------------------------------+
```
According to your wish, you can either save the buffer
content to a file by using `:w [file name]` command or discard
the changes using `:q!` command or you can remove everything
and start typing fresh content by typing `:e!` command. Remember
to hit `<Enter>` key after typing the command.   

Before moving to the next section, get used to Insert Mode and
type different texts to one or more files. Also try the ex
commands mentioned in this section.

To deep dive into our next section, I chose a limerick from 
**Book of Nonsense** by _Edward Lear_. Open vi without any file
name and type the following limerick in it and save it with
the file name `limerick.txt`. In next section, we'll edit
the `limerick.txt` file.
```
+-----------------------------------------------------+
|There was an Old Man on some rocks,                  |
|Who shut his Wife up in a box:                       |
|When she said, "Let me out," he exclaimed, "Without  |
|doubt                                                |
|You will pass all your life in that box."            |
+-----------------------------------------------------+
           Limerick from Book of Nonsense
```

4.3 Operator Commands
---------------------
Now we know how to insert some text in a file using vi editor.
We saved a file with some text in it. Next we'll open the file
and make some changes to it using edit operators. There are some
operators you can use to change text. They are- `c`, `d`,
`y` and `p`.  

To change text, we use `c`, to delete we use `d`, to copy text
(which is known as yanking in vi), we use `y` and to put back 
the copied text, we use `p`. Operators work in conjunction 
with movement commands to make changes. The operator defines
what you want to do and the movement command defines on which 
part of the text you want the change to be made. The part of
the text to be changed is also known as a `Text Object`.
So, in a nutshell, an editing command consists of two parts,
an operator and a movement (Text Object).  

Let's try some hands-on to understand what we are talking
about.

Open the file created in section 4.2 to try editing
commands and make changes to the file.
```
+-----------------------------------------------------+
|$ cd vi-essentials                                   |
|$ vi limerick.txt                                    |
+-----------------------------------------------------+
```
The limerick.txt file's content will be shown- 
```
+-----------------------------------------------------+
|There was an Old Man on some rocks,                  |
|Who shut his Wife up in a box:                       |
|When she said, "Let me out," he exclaimed, "Without  |
|doubt                                                |
|You will pass all your life in that box."            |
+-----------------------------------------------------+
```
### 4.3.1 Change Operator
Let's try to change the "Old Man" in the first 
line to Young Man. To do so, we have to move to the 
first line of the text and move to the word "Old". To 
do so, we need to move to the first line, we can do 
so, by using `j` and `k` commands in Normal mode. Then 
we need to move to the first character of the line, 
which we can achieve by using `0` command. Then, we 
need to move 3 words forward, that can be done using 
`3w` command, then the cursor is in the first character 
of the word Old. Now, let's change the word "Old". The
command `c` in Normal mode works to change the text. 

Remember, operators work on a movement. So, if you
think a little, you can understand that, using `c` 
operator with `w` motion will give you the exact 
result. So, to change the word "Old" we can use `cw` 
here. Once you press `cw`, the word "Old" gets copied 
into copy buffer, it gets deleted from the content 
shown on screen and the editor changes to Insert 
Mode for you to type the replacement for the word 'Old'. 
The screen looks like the following -
```
+-----------------------------------------------------+
|There was an _ Man on some rocks,                    |
|Who shut his Wife up in a box:                       |
|When she said, "Let me out," he exclaimed, "Without  |
|doubt                                                |
|You will pass all your life in that box."            |
+-----------------------------------------------------+
```
Now you can type the new word-
```
+-----------------------------------------------------+
|There was an Young_ Man on some rocks,               |
|Who shut his Wife up in a box:                       |
|When she said, "Let me out," he exclaimed, "Without  |
|doubt                                                |
|You will pass all your life in that box."            |
+-----------------------------------------------------+
```

Once you are done, you can hit `<Esc>` or `Ctrl+[` key to 
be back to normal mode.
The same way, you can use `b`, `h`, `l`, `$`, `0`, `e`, `^`,
`W`, `B`, `E` etc.  movements with the `c` command. 
Remember, c commands puts you in Insert Mode.
      
### 4.3.2 Delete Operator
The delete operator in vi editor is `d`.
`d` operator works the same way `c` operator
works, except for the fact that, it does not put you 
in Insert Mode. Let's delete the word "Young" from the
content. To do that, move the cursor to the starting 
of the word "Young" and hit `dw`. It will delete the 
word and the following space and the cursor will blink
just below the letter 'M'. The word "Young" gets copied 
into copy buffer.
```
+-----------------------------------------------------+
|There was an Man on some rocks,                      |
|Who shut his Wife up in a box:                       |
|When she said, "Let me out," he exclaimed, "Without  |
|doubt                                                |
|You will pass all your life in that box."            |
+-----------------------------------------------------+
```
Similar to `c` operator, `d` operator also works on `b`,
`h`, `l`, `$`,`0`,`e`,`^` etc. movements.

### 4.3.3 Yank Operator
In vi terminology, copying is known as 'yanking'.
Yanking means, copy a text for future use without
deleting the original text. To yank in vi, we use `y`
operator.
The `y` operator works like `d` operator except it does 
not delete the original text. It just copies it. Now,
let's try to copy the word "Man". The cursor now already 
blinks under Man, so, if we press `yw`, it will copy 
the word "Man" into buffer -
```
+-----------------------------------------------------+
|There was an Man on some rocks,                      |
|Who shut his Wife up in a box:                       |
|When she said, "Let me out," he exclaimed, "Without  |
|doubt                                                |
|You will pass all your life in that box."            |
+-----------------------------------------------------+
```
Notice that, there is no change in the text. It means,
that `y` operator did not change any text, instead, it 
just copied the content into buffer. 
      
      
### 4.3.4 Put Operator
Now we know that how to copy, cut and change text. We
also know that, all the three change operators copy
the text object in a buffer (which we called as Copy 
Buffer, aka Unnamed Default Buffer). vi editor also 
allows to paste the copied text object. In vi 
terminology, this is known as 'put'. The operator to put
text back is `p`. When you type `p` in Normal mode, it 
will paste the text from buffer in the cursor location.
If you type `P`, it will paste the text from buffer on 
the left of the cursor.

Now we'll paste (put) the copied text after the word
"some", so, we'll move the cursor after the word "some" 
and press `p`. The result would be the following -
```
+-----------------------------------------------------+
|There was an Man on some Man rocks,                  |
|Who shut his Wife up in a box:                       |
|When she said, "Let me out," he exclaimed, "Without  |
|doubt                                                |
|You will pass all your life in that box."            |
+-----------------------------------------------------+
```   
If we now try to paste the same word just before the
word "Who" on the second line, we'll move the cursor to
the first of the second line by using `+` and press `P`.
The text shold look like the following -
```
+-----------------------------------------------------+
|There was an Man on some Man rocks,                  |
|Man Who shut his Wife up in a box:                   |
|When she said, "Let me out," he exclaimed, "Without  |
|doubt                                                |
|You will pass all your life in that box."            |
+-----------------------------------------------------+
```
4.4 Operator with count
-----------------------
Edit operators work on text objects (which are text based on
the cursor movement). So, if you want to delete 2 words on
the right of the cursor, you type `d2w` or to delete 2
characters on the left of cursor, you use `d2h`. Similarly it
works with `c` and `y` as well. That is the operator is 
performing an edit based on repeated motion.  

However, you can also perform repeated operations as
well. So, to delete 2 characters on the left of cursor you
can use `2dh` instead of `d2h`.
So, `d2h` and `2dh` works the same. The first combination means,
delete 2 characters on the left of the cursor while the
second one means, delete a character on the left of the
cursor 2 times. Same goes for `c` and `y` as well. So, `d2h` 
and `2dh` work same way, `3ch` and `c3h` work same way, `2yw`
and `y2w` work same way.  

You can also combine both. So, `2d3h` is also a valid change
command. This means, delete 3 characters on the left of the
cursor 2 times. So, a total 6 characters on the left from
the cursor position will be deleted. Similarly `3c2w`,
`4y3w` etc. also are valid commands.

4.5 Whole Line Editing
----------------------
In some cases, you also need to change a whole line of text,
or you need to copy a whole line and paste it back in some
other location of the file. To do this, you can move to the
line you want to change or copy, press `0` which will move the
cursor to the first of the line and press `d$`, `c$` or
`y$`. This will do the job but is a little bit of extra work.
vi editor solves this problem by using shorcut. You can move to the 
line you want to change or copy and press `cc` or `dd` or
`yy`. These commands will perform the exact same task.  

If you copied or changed or deleted a whole line using `cc`
or `dd` or `yy`, `p` operator works in a different way. If a
whole line has been copied in buffer and you use `p` command
after that, it pastes the whole line just below the current
line. If you press `P`, then the line is pasted above the
current line.

4.6 Summary
------------
These were pretty much all the basic editing staffs to be
performed in vi editor. You should practice these as much 
as possible as these form the base of using vi editor. 

For your reference, here we put another table for easy
recapitulation -
```
+===========================================================+
|                  Edit commands                            |
|===========================================================|
|Text object          | Change     | Delete     | Copy      |
|---------------------|------------|------------|-----------|
|One word forward     | cw         | dw         | yw        |
|-----------------------------------------------------------|
|Two words, not       | 2cW or     | 2dW or     | 2yW or    |
|counting punctuation | c2W        | d2W        | y2W       |
|-----------------------------------------------------------|
|Three words back     | 3cb or     | 3db or     | 3yb or    |
|                     | c3b        | d3b        | y3b       |
|-----------------------------------------------------------|
|Six words back       | 3c2b or c6b| 3d2b or d6b|3y2b or y6b|
|                     |      or    |      or    |     or    |
|                     | 2c3b or 6cb| 2d3b or 6db|2y3b or 6yb|
|-----------------------------------------------------------|
|Six words forward    | 3c2w or c6w| 3d2w or d6w|3y2w or y6w|
|                     |      or    |      or    |     or    |
|                     | 2c3w or 6cw| 2d3w or 6dw|2y3w or 6yw|
|-----------------------------------------------------------|
|To end of line       | c$         | d$         | y$        |
|-----------------------------------------------------------|
|To beginning of line | c0         | d0         | y0        |
|-----------------------------------------------------------|
|One line             | cc or 0c$  | dd or 0d$  | yy or 0y$ |
+-----------------------------------------------------------+
```
For saving or discrading changes, use the following ex 
commands -
```
+-----------------------------------------------------------+
|  Command      |   Action                                  |
|---------------|-------------------------------------------|
|:w [file name] | This is Save Command. A new file is       |
|               | created with name 'file name' and the     |
|               | buffer content is saved in the file.      |
|               | If the file exists, it won't allow        |
|               | you to save.                              |
|---------------|-------------------------------------------|
|:w! [file name]| If the file exists with name 'file name', |
|               | the file is overwritten with the content  |
|               | otherwise, a new file is created. Please  |
|               | be careful while using this command. Im-  |
|               | proper use of this can loss existing data |
|---------------|-------------------------------------------|
|:q             | This is Quit command. So, it will try to  |
|               | quit the editor. But will show an error   |
|               | mentioning that the  content of the       |
|               | buffer is not saved. If there is no change|
|               | It quits the edior and returns to shell   |
|---------------|-------------------------------------------|
|:wq            | Combined Save and Quit Command. So, if vi |
|               | is opened with no file input, it will try |
|               | to save the content but as no             |
|               | file name is mentioned, it cannot save    |
|               | the buffer content and will show error.   |
|               | If vi is opened with an existing file, it |
|               | will save the changes to the file. If vi  |
|               | If vi is opened with an input as a file   |
|               | name that does not exist, the file is     |
|               | created and the content is saved into file|
|---------------|-------------------------------------------|
|:wq [file name]| Combined Save and Quit Command. So, the   |
|               | content will be saved to file named 'file |
|               | name' and quit the editor.                |
|---------------|-------------------------------------------|
|:e!            | This command is issued to discard the     |
|               | changes. As we started with empty file,   | 
|               | a blank screen will be shown discarding   |
|               | all the changes.                          |
|---------------|-------------------------------------------|
|:q!            | Will discard the changes and exit vi      |
+-----------------------------------------------------------+
```
`p` pastes the content of buffer in the cursor location, on the
other hand `P` pastes the contents of buffer on the left of 
the cursor. If you copied whole line using `cc` or `dd` or
`yy` then `p` pastes the line from buffer below the current line and
`P` pastes the line from buffer above the current line.  

Till now we have covered all the basic movement and editing
commands. You can definitely save your day on a remote
machine connected through `ssh` using this set of commands.
Though the editing will neither be fast nor be efficient,
you will at least be able to complete. So, you can stop
here if you want.  

On the other hand, if your intention is to employ `vi` for
your day to day editing needs, you need speed. Which we'll
see how to achieve in our upcoming chapters, where we'll
talk about some shortcuts, some advance movements and some
`ex` commands which will make your editing a lot faster and
more conventient.



