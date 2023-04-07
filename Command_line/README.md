# Practice in the Terminal
### What is the command line, how does it work and how do I get to one
* A command line, or terminal, is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text

* If you're on a Mac then you'll find the program Terminal under Applications -> Utilities. An easy way to get to it is the key combination 'command + space' which will bring up Spotlight, then start typing Terminal and it will soon show up.
If on Linux then you will probably find it in Applications -> System or Applications -> Utilities. Alternatively you may be able to 'right-click' on the desktop and there may be an option 'Open in terminal'.
If you are on Windows and intend to remotely log into another machine then you will need an SSH client. A rather good one is Putty (free) .
--------
### Basic Navigation - An introduction to the Linux directory system and how to get around it.

* pwd  
Print Working Directory - ie. Where are we currently.
* ls  
List the contents of a directory.
* cd  
Change Directories - ie. move to another directory.
* Relative path  
A file or directory location relative to where we currently are in the file system.
* Absolute path   
A file or directory location in relation to the root of the file system.
----------
### More About Files - Find out some interesting characteristics of files and directories in a Linux environment.
* file.exe - an executable file, or program.
* file.txt - a plain text file.
* file.png, file.gif, file.jpg - an image
* Linux is Case Sensitive
* a space on the command line is how we separate items, You may use either single or double quotes. Anything inside quotes is considered a single item or use backslash ( \ ). What the backslash does is escape (or nullify) the special meaning of the next character.
* file
obtain information about what type of file a file or directory is.
* ls -a
List the contents of a directory, including hidden files.
* Everything is a file under Linux
Even directories.

### Manual Pages - Learn how to make the most of the Linux commands you are learning.
Look up the manual page for a particular command:

``` 
man <command>
```
Do a keyword search for all manual pages containing the given search term:
```
man -k <search term>
```
Within a manual page, perform a search for 'term'
```
/<term>
```
After performing a search within a manual page, select the next found item.
```
n
```
 * To exit the man pages press 'q' for quit.

### File Manipulation - How to make, remove, rename, copy and move files and directories.
* Making a Directory
```
mkdir [options] <Directory>

```
* Removing a Directory
```
rmdir [options] <Directory>

```
* Creating a Blank File
```
touch [options] <filename>

```
* Copying a File or Directory
```
cp [options] <source> <destination>

```
* Moving a File or Directory
```
mv [options] <source> <destination>

```
### Removing a File (and non empty Directories)
```
rm [options] <file>
```
* No undo
The Linux command line does not have an undo feature. Perform destructive actions carefully.
* Command line options
Most commands have many useful command line options. Make sure you skim the man page for new commands so you are familiar with what they can do and what is available.

### [Cheat Sheet - A quick reference for the main points covered in this tutorial.](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)








