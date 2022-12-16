## Reading Notes 2: The Bash Command Line

### The Command Line

According to [Ryans Tutorials: The Command Line!](https://ryanstutorials.net/linuxtutorial/commandline.php), a terminal/command line is a "text based interface to the system". It allows to enter commands by typing, and will give results back as text. It starts with a prompt, since I'm using Ubuntu, the prompt as I open it looks like this:

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

### Basic Navigation[^2]

#### pwd

The **pwd** (Print Working Dierectory) lets you know the current working directory you are in.

<img width="608" alt="image" src="https://user-images.githubusercontent.com/113204667/207969826-4ff08cc3-dbb3-450c-8b0d-b3ecca97f850.png">

#### ls

The **ls** (list) states or lists the files or directories on your current location.

<img width="526" alt="image" src="https://user-images.githubusercontent.com/113204667/207970837-ca0c61df-3717-4a27-ad5c-02b5ff8a0f26.png">

#### ls -l

The **ls -l** includes long lists, the *d* in *drwxr-xr-x* indicates that the file is a *directory*, if *-* then it is a normal file. The next 9 characters indicates the permissions for that file/directory. The next field indicates the number blocks, while the next one indicates the owner, and then "the group the file or directory belongs to[^2]". The *4096* is the file size, then the date and time it was modified/created, and then the filename/directory name.

<img width="529" alt="image" src="https://user-images.githubusercontent.com/113204667/207971621-4fbee4ad-577b-485d-8829-d3add3af5632.png">

#### ls /etc

The command **ls /etc** lists the directories' contents (not including the directory name, but just the contents).

#### ls -l /etc

The command **ls -l /etc** includes a long listing of the directories' contents.

#### Paths: Absolute and Realtive

The *path* lets you get to a specific directory or file[^2]. Two types of paths are **absolute** and **relative**. The **/** indicates the root directory.

An example of *relative path* is:

<img width="596" alt="image" src="https://user-images.githubusercontent.com/113204667/207975120-1cf5a960-d8c2-4356-a040-b125736c719a.png">

An example of absolute path is:

<img width="521" alt="image" src="https://user-images.githubusercontent.com/113204667/207975564-83d10209-6bcd-40db-9d41-9cd9d42888ab.png">

#### Other building blocks on Paths[^2]

We can use the following to refer to a location:

- **~** and **cd (without arguments)** -> is a shortcut for home directory
- **.** -> is a "reference to your current directory[^2]"
- **..** -> is a "reference to the parent directory[^2]"
- **cd /h + Tab** -> invokes an auto-complete of directory that starts with "h", if Tab is hit once again, it will show the next possibilities

The **cd** stands for change directories.

<img width="567" alt="image" src="https://user-images.githubusercontent.com/113204667/207980031-61388fef-db03-4664-aeed-c5f1d4d6604d.png">


### More About Files[^3]

With linux, **everything is a file**, including text file, directory, keyboard - the system that reads from, and monitor - the system that writes to[^3]. A file extension is usually made up of 2-4 characters. This extension states the type of file, such as:

- **file.txt** as a plain text file
- **file.exe** as executable program/file
- **file.png, file.jpg, file.gif** as image

Another important thing to remember is that, linux, is **case sensitive**. It is possible to have more than one file with same name as long as the characters/letters are of different case[^3]. For example sample.txt is different from Sample.txt, or SAMPLE.txt; these three files, although same filename, can exist due to they all differ in casing.

**Spaces** in directory and file are ok, however, it is not advised to use space in filenames or directory names due to spaces are used to separate items in the command line. If the filename includes spaces, one must use quotes or escape characters to access it, such as[^3]:

- *cd 'Sample Text'* 
- *cd Sample\Text*

Below will not work:
cd Holiday Photos

The **hidden files and directories** are usually stored with a name starting at **"."** (full stop). Such configuration files are hidden to not "get in the way of the user doing their everyday tasks[^3]".


### Manual Pages[^4]



References:
[^1]: [Ryans Tutorials: The Command Line!](https://ryanstutorials.net/linuxtutorial/commandline.php)
[^2]: [Ryans Tutorials: Basic Navigation](https://ryanstutorials.net/linuxtutorial/navigation.php)
[^3]: [Ryans Tutorials: More About Files!](https://ryanstutorials.net/linuxtutorial/aboutfiles.php)
[^4]: [Ryans Tutorials: Manual Pages!](https://ryanstutorials.net/linuxtutorial/manual.php)
