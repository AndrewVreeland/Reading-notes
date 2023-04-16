# [The Command Line](https://ryanstutorials.net/linuxtutorial/commandline.php) - What is it, how does it work and how do I get to one

1. The command Line exsists inside of your terminal this is where you give commands to your computer. you will then be returned information or errors depending on what command you put in.

## [Basic Navigation](https://ryanstutorials.net/linuxtutorial/navigation.php) - An introduction to the Linux directory system and how to get around it

1. pwd: Print Working Directory, tells you where you are in your file system
  
2. ls: list, provides a list within your current position that shows what directories are available

3. /: this symbol is the ROOT

4. ~: shortcut for the home directory

5. ..: previous directory.

6. cd: change directory ex. cd.. moves back one directoy

### Important Concepts

#### Relative path

A file or directory location relative to where we currently are in the file system.

#### Absolute path

A file or directory location in relation to the root of the file system.

## [More About Files](https://ryanstutorials.net/linuxtutorial/aboutfiles.php) - Find out some interesting characteristics of files and directories in a Linux environment

1. file.exe - an executable file, or program.
2. file.txt - a plain text file.
3. file.png, file.gif, file.jpg - an image.
4. files that start with a . are hidden
5. ls -a: List the contents of a directory, including hidden files.

### Important Concepts

#### Everything is a file under Linux

Even directories.

#### Linux is an extensionless system

Files can have any extension they like or none at all.

#### Linux is case sensitive

Beware of silly typos.

## [Manual Pages](https://ryanstutorials.net/linuxtutorial/manual.php) - Learn how to make the most of the Linux commands you are learning

1. The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept.

2. man <command> Look up the manual page for a particular command.

3. man -k <search term> Do a keyword search for all manual pages containing the given search term.

4. /<term> Within a manual page, perform a search for 'term'

5. n, After performing a search within a manual page, select the next found item.

## [File Manipulation](https://ryanstutorials.net/linuxtutorial/filemanipulation.php) - How to make, remove, rename, copy and move files and directories

1. mkdir: make directory

2. rmdir: remove directory

3. tocuh: creates a file

4. cp: copies file or directory 

5. mv: moves file or directory

6. RENAME FILE EXAMPLE: mv linuxtutorialwork/testdir /home/ryan/linuxtutorialwork/fred

7. rm: remove files and non empty directories

### IMPORTANT CONCEPTS 

#### No undo

The Linux command line does not have an undo feature. Perform destructive actions 
carefully.

#### Command line options

Most commands have many useful command line options. Make sure you skim the man page for new commands so you are familiar with what they can do and what is available.

## [Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php) - A quick reference for the main points covered in this tutorial
