
# Command line

Table of contents

- [Theory](#theory)
    - [Help](#help)
    - [Parameters](#parameters)
    - [Flags](#flags)
    - [Autocomplete](#autocomplete)
    - [Clear](#clear)
    - [Signals](#signals)
- [Commands](#commands)
    - [mkdir](#mkdir)
    - [rm](#rm)
    - [cp](#rm)
    - [mv](#rm)
    - [ps](#rm)
    - [sleep](#rm)
    - [shutdown](#rm)
- [Environment variables](#environment-variables)

## Theory

When you open a command line you are essentially looking at a REPL or Read Evaluate Print Loop and is used to navigate around your computer, create folders and files, edit or delete files, make network calls, inspect the computer parameters and much more. When you are using REPL you are feeding one command at a time to the system and getting the result back. 

### Help
Remembering all the commands and it’s parameters can be challenging and therefore the help commands comes in handy. To use the help functionality you simply append –help to the command. While this works fine in Linux system in Windows you can append `/?` To get the same behaviour E.g.
```shell
# Linux
color –-help

# Windows
color /?
```
### Parameters
The parameters are the value that you feed to the functions, you can use the help commands to get what parameters the command accept. E.g.
```shell
cd ..
```
In this case CD is the command and `..` is the parameters. 
```shell
echo hi
```
### Flags
Flags like parameters allow to pass values into the command but in a more intelligent way. Flags help the command understand what you want it to do. 
```shell
# Linux
ls -l

# Windows
dir /b
```

### Autocomplete

Most command line offers autocomplete to accelerate the process of writing commands,
for example if you start writing `dir s` and press tab, it will automatically 
complete with the closest result in this case it will be `dir source`

### Clear

When you screen is filled with errors you can easily clear them out with the clear
command

```shell
# Linux
clear

# Windows
cls
```

### Signals

#### CTRL + C

Interrupts the execution of a command

CTRL + D

Closes the bash session at least in Linux


## Commands

### mkdir

Creates a new folder in the current directory

```shell
mkdir test
```

### rm

Removes the specified folder or file.

```shell
rm test
```

### cp

Copy the specified file into the specified folder or file 

```shell
# Copy to folder
cp test.txt test

# Copy to new file
cp test.txt my-new-copy.txt
```

### mv

Move the file to a new destination, it can also be used to rename the file

```shell
mv test.txt ./test

mv test.txt new-name.txt
```

### ps

Shows all the current processes

```shell
ps
```

### sleep

Sleep

```shell
sleep 100
```
### shutdown

```shell
shutdown /s /f /t 300 /c "Turning off"

# To stop the shutdown
shutdown /a
```




## Environment variables

Environment variables allow you to store temporarily some data

```shell

# Windows
$TEST=1

echo "My number is $TEST"
```
