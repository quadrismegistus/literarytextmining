# (1C) The Terminal [PRACTICUM]

## Follow the maze!

### Terminal adventures

Imagine you're in an old text adventure game, like [Adventure (1977)](https://en.wikipedia.org/wiki/Interactive_fiction#Adventure):

<img src="https://upload.wikimedia.org/wikipedia/commons/2/25/ADVENT_--_Crowther_Woods.png" width=500>

These games were popular in the late 1970s and 1980s. Today's practicum is written in their spirit.

### Setup

First, enter the folder of the mazes:

```
cd ~/literarytextmining/01_setup/01C_TODO_the_terminal
```

### Assignment

You see before you three "mazes," each of which is a folder.
(If you type `ls`, you should see: `README.md	maze1		maze2		maze3`).

Inside each of these mazes is an unknown number of other folders. Buried somewhere in these nested folders is a file called "finish.txt". We want to find these the "finish.txt" file for each of the three mazes, and read what's inside them.

Use `cd` and `ls` to navigate through each maze.  When you find "finish.txt", print out its contents using `cat.` We learned all of this in our module, [(1C) The Terminal](01C_the_terminal).

We'll do the first maze together. The second and third will be done on your own, in class or at home, time depending.

The final assignment is to paste the contents of maze3's "finish.txt" into Canvas.

### Maze 1

Let's enter the first maze.

```
# enter the folder of the mazes
cd ~/literarytextmining/01_setup/01C_TODO_the_terminal

# enter maze 1
cd maze1
```

We're in. What's here? Let's use `ls`:

```
ls
```

This should return:

```
door1	door2
```

Let's pick a door to go into:

```
cd door1   # move into the first door
ls         # list what's inside the first door
```

This should return nothing at all. "door1" is empty! Curses!

Well, let's take stock of where we are. Where are we again?

```
pwd
```

This should return something like:

```
/Users/ryan/literarytextmining/01_setup/01C_TODO_the_terminal/maze1/door1
```

Great: we're inside the first door of the first maze (`.../maze1/door1`). Now, how do we go back "up" again?

```
cd ..      # go up one directory
ls         # list what's here again
```

This should bring us back to:

```
door1	door2
```

Let's try the second door:

```
cd door2   # move into the second door
ls         # list what's inside the second door
```

What's in the second door? We should see:

```
finish.txt
```

Aha! We found it! Now, how do we read it again?

```
cat finish.txt
```

We use "cat" to print out the contents of a file. And now we should see:

```
           __..--''``---....___   _..._    __
 /// //_.-'    .-/";  `        ``<._  ``.''_ `. / // /
///_.-' _..--.'_    \                    `( ) ) // //
/ (_..-' // (< _     ;_..__               ; `' / ///
 / // // //  `-._,_)' // / ``--...____..-' /// / //
```

A sleeping cat! Probably because this maze was so easy. Try two harder ones on your own!

### Maze 2

Try on your own during class. Ask for help if you need it.

### Maze 3

Try on your own at home. Paste what you find in maze3's "finish.txt" onto the assignment in Canvas.