# (1C) The Terminal

## Introduction

Before the Graphical User Interfaces (GUI) of the present day, the "terminal" is how a human interacted with the digital computer. First developed in Berlin in 1941, terminals remained the dominant interface system until GUIs became more popular in the 1980s and 90s. Microsoft, for example, released its graphic "Windows" operating system in 1981, following its earlier "MS-DOS."

## Setting up the Terminal

1. Open the Terminal.
	* On Mac, go to: Applications > Utilities > Terminal.
	
	* On Windows: Start > All Programs > Accessories > Command Prompt
		* Windows users: consider installing a better terminal app, like [cmder](https://cmder.net/).

2. Customize the appearance (optional)
	* On Mac:
		* Go to preferences (Cmd + comma)
		* Double click theme ("Homebrew" recommended for fans of The Matrix)
		* Click "Default"
		* Click Color & Effects
		* Lower opacity (helps for typing lines onto the Terminal from another source, which is made partly visible behind the terminal screen)
	* On Windows:
		* If using [cmder](https://cmder.net/) for a terminal:
			* Go to settings (Win + Alt + p)
			* Go to Features > Transparency
			* Increase transparency


## Navigating folders

Memorize these basic commands.

### (1) "cd": change directory

When you open the Terminal, you open it to a particular *place* -- a particular "directory" or "folder" -- in the file system, just as every time you open a Finder window on a Mac, you are in a particular directory or folder.

```
cd        # go to your home folder (e.g. /Users/ryan)
cd ~      # go to your home folder (e.g. /Users/ryan)
pwd       # print working directory (where are we now?)
```
You should see the **"path"** to your directory. I see: ```/Users/ryan```

Let's change directory again:

```
cd ..     # go up one directory
pwd       # print working directory
```

You should now see the path to the directory above the one we were in. I see: ```/Users```

To be above means to "contain." An analogy: If we were first in Room 240-110, to go "up" means to go to Building 240, which contains Room 240-110.

Let's go up one more time.

```
cd ..     # go up one directory
pwd       # print working directory
```

We should now be at the **"root" directory**, the directory that contains all other directories, which is known as: ```/```

To review, here are a few magic names for folders:

* `~`: your home folder
* `..`: the folder above the one we're in now
* `.`: the folder we're in right now
* `/`: the root folder of the entire file system

But let's stop using these magic names and go to a normal, named folder. Let's now move directly to our class repository folder, which we [installed in module (1B)](https://github.com/quadrismegistus/literarytextmining/blob/master/01_setup/1A_installation_instructions.md#2-clone-class-repository):

```
cd ~/literarytextmining
```

Great! (Hacker voice: "We're in.") But what's in there?


### (2) "ls": list contents of directory

But how do we know what's in a directory? Using "ls."

```
cd ~/literarytextmining    # go to our class folder
ls                         # list contents of home folder
```

You should see the filenames of every file in our course folder. To display in more detail:

```
ls -l     # list contents of home folder in more detail
```

You should see something like this:

```
total 104
drwxr-xr-x@ 4 ryan  staff    128 Mar 30 09:41 01_setup
-rw-r--r--@ 1 ryan  staff  15129 Mar 29 23:29 README.md
drwxr-xr-x@ 3 ryan  staff     96 Mar 29 16:17 corpora
```

These represent ([source](https://unix.stackexchange.com/a/140944)):

```
-rw-r--r--@    1    ryan  staff   15129    Mar 29 23:29 README.md
?UUUGGGOOOS   00  UUUUUU GGGGGG   #####    ^-- date stamp and file name are obvious ;-)
^ ^  ^  ^ ^    ^      ^      ^    ^
| |  |  | |    |      |      |    \--- File Size
| |  |  | |    |      |      \-------- Group Name (for example, Users, Administrators, etc)
| |  |  | |    |      \--------------- Owner Acct
| |  |  | |    \---------------------- Link count (what constitutes a "link" here varies)
| |  |  | \--------------------------- Alternative Access (blank means none defined, anything else varies)
| \--\--\----------------------------- Read, Write and Special access modes for [U]ser, [G]roup, and [O]thers (everyone else)
\------------------------------------- File type flag
```

You can sort this list by the last modified:

```
ls -ltr
    ^^^
    |||
    ||\------ reverse the sort (so newest on bottom)
    |\---- sort by time
    \-- show in list format 
```  

The four lines above will become sorted by their date of last modification:

```
total 104
drwxr-xr-x@ 3 ryan  staff     96 Mar 29 16:17 corpora
-rw-r--r--@ 1 ryan  staff  15129 Mar 29 23:29 README.md
drwxr-xr-x@ 4 ryan  staff    128 Mar 30 09:46 01_setup
```

### (3) "mkdir": Make a directory

We can make folders by using "mkdir" command. Let's make a "workspace" folder in our class repository.

```
cd ~/literarytextmining    # go to our class folder
mkdir workspace            # make a folder called 'workspace'
cd workspace               # change directory to 'workspace'
pwd                        # where are we now?
```

You should see something like: ```/Users/ryan/literarytextmining/workspace```

This folder will be ignored by github (set in the file ```.gitignore```), so do with it as you will.

Let's make one more folder:

```
cd ~/literarytextmining    # go to our class folder
cd workspace               # change directory to 'workspace'
mkdir terminal_practice    # make a folder in the workspace called 'terminal_practice'
cd terminal_practice       # move into the 'terminal_practice' folder
```


## Reading files

### (4) "cat": print the entire contents of a file

To read files, use "cat":

```
cd ~/literarytextmining    # go to course folder
cat README.md              # print the contents of the syllabus
cd 01_setup                # go into the first module's folder
cat 1C_the_terminal.md     # print this terminal introduction file
```

### (5) "less": show part of the contents of a file

To read files bit by bit, which is useful for large files, use "less":

```
cd ~/literarytextmining    # go to course folder
less README.md             # show first part of syllabus
```

Once inside of `less`, hit:

* "Enter" to scroll down a line
* "Page Down" (on Mac: fn + down arrow) to go down a page;
* "q" to quit

### (6) "grep": search files

To search a file for a specific word, use grep. The syntax is: `grep "PATTERN" FILE`. For example:

```
cd ~/literarytextmining    # go to course folder
grep "4/4" README.md       # search syllabus for mentions of the phrase "4/4"
```

This should print out the lines mentioning "4/4". Something like this:

```
|      | 2     | Th  | 4/4  | (2) Corpora                     | (2A) Introduction to corpora; (2B) Building your own corpus   | Read: ToO, 7-25 [“Monday," ch. 1-3]      |
```

Other options (advanced):

```
grep -i terminal README.md               # search for 'terminal' case-insensitive
grep --color=auto terminal README.md     # color results
grep -w "4/2" README.md                  # search only for whole word matches
grep -R terminal 01_setup                # search
```

For a more in-depth introduction to grep, [see here](https://opensourceforu.com/2012/06/beginners-guide-gnu-grep-basics/).

## Practicum

[See here for the practicum for this module](1C_the_terminal_TODO/README.md).