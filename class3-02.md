## Reading Notes 2: The Bash Command Line

### The Command Line

According to [^1]: [Ryans Tutorials: The Command Line!](https://ryanstutorials.net/linuxtutorial/commandline.php), a terminal/command line is a "text based interface to the system". It allows to enter commands by typing, and will give results back as text. It starts with a prompt, since I'm using Ubuntu, the prompt as I open it looks like this:

**issa29@DESKTOP-N7B8RN9:~$**

Based on the image below, as stated in [Ryans Tutorials: The Command Line!](https://ryanstutorials.net/linuxtutorial/commandline.php):

Line1 = the prompt **issa29@DESKTOP-N7B8RN9:~$**, followed by the command **ls**, and the command line **-l /home/issa29**, these three are separated by spaces. the command *ls* is used to list files, while *-l* is an *option* "used to modify the behaviour of the command[^1]".

Lines 2-5 = the output or the results after executing the command.

Line 6 = back with the prompt again

<img width="730" alt="image" src="https://user-images.githubusercontent.com/113204667/207963763-6d84b94f-4b4d-4c41-98b2-e38318cae298.png">

#### Opening a terminal[^1]:

For Mac Users:
Applications > Utilities > Terminal

For Linux:
Applications > Utilities > Terminal **or**
Applications > System > Terminal

For Windows Users:
(Mine is) Apps > Installed Apps > Terminal
[Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html) is another way if user wants to "remotely log into another machine then you will need an SSH client"[^1].

#### Shell, Bash

A **shell** is a part of OS that shows how the terminal behaves after running/executing the commands; **bash (Bourne agaian shell)** is one of the most common *shells* [^1]. Typing the **echo $SHELL** on the terminal displays the shell you are using, as shown in the image below:

<img width="563" alt="image" src="https://user-images.githubusercontent.com/113204667/207968282-a9ec96e2-3fd7-4c42-97c3-1e10235ef04f.png">

#### Shortcuts

The commands entered are usually stored in a history, one can use the arrow keys up and down to scroll the history, instead of typing the same command again[^1].


References:
[^1]: [Ryans Tutorials: The Command Line!](https://ryanstutorials.net/linuxtutorial/commandline.php)
