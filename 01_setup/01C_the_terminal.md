# The Terminal

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

Let's now move directly to our class repository folder, which we [installed in module (1B)](https://github.com/quadrismegistus/literarytextmining_spring2019/blob/master/01_setup/01A_installation_instructions.md#2-clone-class-repository):

```
cd ~/literarytextmining_spring2019
```

Great! (Hacker voice: "We're in.") But what's in there?


### (2) "ls": list contents of directory

But how do we know what's in a directory? Using "ls."

```
cd        # go to your home folder (e.g. /Users/ryan)
pwd       # check we're in the home folder
ls        # list contents of home folder
```

You should see the filenames of every file in your home directory. They are likely in multiple columns, depending on the size of the Terminal window. To display in more detail:

```
ls -l     # list contents of home folder in more detail
```

You should see a bunch of stuff printed out. Here's an example set of four lines:

```
drwx------+    4 ryan  staff        128 Mar 29 18:16 Desktop
drwxr-xr-x+  236 ryan  staff       7552 Feb  8 16:08 Documents
drwxr-xr-x+  439 ryan  staff      14048 Mar 29 18:10 Downloads
drwx------@   11 ryan  staff        352 Dec  7 20:49 Dropbox
```

These represent ([source](https://unix.stackexchange.com/a/140944)):

```
drwx------+    4    ryan  staff  128    Mar 29 18:16 Desktop
?UUUGGGOOOS   00  UUUUUU GGGGGG ####    ^-- date stamp and file name are obvious ;-)
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
drwx------@   11 ryan  staff        352 Dec  7 20:49 Dropbox
drwxr-xr-x+  236 ryan  staff       7552 Feb  8 16:08 Documents
drwxr-xr-x+  439 ryan  staff      14048 Mar 29 18:10 Downloads
drwx------+    4 ryan  staff        128 Mar 29 18:16 Desktop
```

### (3) "mkdir": Make a directory

We can make folders by using "mkdir" command.

```
cd                  # go to home folder
mkdir test_folder   # make a folder called 'test_folder'
cd test_folder      # change directory to 'test_folder'
pwd                 # print path to where we are now (our working directory)
ls                  # list contents of folder
```

## Reading and writing files

### (4) "vi": create and edit files

To create and edit files, use the "vi" command (advanced: use ["emacs"](https://www.digitalocean.com/community/tutorials/how-to-use-the-emacs-editor-in-linux)).

["vi" is a [text editor developed for UNIX in 1976](https://en.wikipedia.org/wiki/Vi). A major new implementation of vi was [published as "vim" in 1991](https://en.wikipedia.org/wiki/Vim_(text_editor)), which is now used in most operating systems when one invokes "vi".]

For example:


```
cd test_folder      # navigate into our test folder [created in (3)]
vi testing.txt      # edit the file 'testing.text' (create if needed)
```

We are now inside the "vi" editor. This is an old but very sophisticated piece of software, but we will focus on only three commands.

* Type ```i``` to enter **insert** mode
	* Now type some text. Like: "hello world"
	* Now hit escape to escape INSERT mode

* Type ```:w``` to **save** the file

* Type ```:q``` to **quit** vi

For a more thorough introduction, [see this guide](https://www.linux.com/learn/vim-101-beginners-guide-vim).

### (5) "cat": print the entire contents of a file

To read files, use "cat":

```
cat testing.txt      # print the contents of testing.text
```
Should return ```Hello world```, or whatever we typed into testing.txt in (4).

### (6) "less": show part of the contents of a file

To read files bit by bit, which is useful for large files, use "less":

```
less testing.text
```

Should return:

```Hello world
testing.txt (END)
```

This will come in handy later.


## Advanced

### (7) "grep": search files

```
grep
