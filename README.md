
# Table of Contents
1. [CommonCommands](#CommonCommands)
    1. [PWD](#PWD)
    2. [LS](#LS)
    3. [CD](#CD)
    4. [MV](#MV)
    5. [RM](#RM)
3. [DirBister](#DirBuster)
4. [Gobuster](#Gobuster)
5. [Nikto](#Nikto)
6. [NC](#NC)
    1. [Listen_For_Reverse_Shell](#Listen_For_Reverse_Shell)
7. [Hydra](#Hydra)
    1. [Check_if_Content_is_not_on_page](#Check_if_Content_is_not_on_page)
    1. [Check_for_redirect](#Check_for_redirect)
8. [Usefull Linux Commands](#Usefull_Linux_Commands)

# Color

```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```

# Syntax highliting

```bash
  echo "hello world"
``` 

```python3.9
    import os

    os.system("ls -la")
```

# DV2
## CommonCommands
### PWD
```diff
pwd #shows current dir  
```
### LS
```diff
ls #shows files in a folder
+ -l # use a long listing format
+ -a # list all
+ - R #list all subfolders
! drwx rwx rwx # d = dir;
```
### CD
```diff
cd "Path"
+ ~ = home dir
+ .. = dir "over" current dir
+ . = current dir
```
### MV
Move
```diff
mv <dir/filename> </newDir/newFilename>
+ -d #for directory
```
### RM
Remove
```diff
rm <filename>
+ -d #for directory
```
### CP
Copy
```diff
cp <filename>
+ -d #for directory
```
### HISTORY
```diff
@@ history #shows command history @@
```
### CAT
```diff
cat
```
### TOUCH (creates a file)
```diff
touch <filename>
```
### MKDIR
```diff
mkdir <dirname>
```

### .
```diff
.programmname #starts a programm
ctrl+c #stops a programm
```
### PS
```diff
ps #shows processes on current user
+ -ef #shows all processes

UID = user
PID = Process ID
PPID = if a process started a new Process
TIME = running time
STIME =
CMD = the command which started the Process
[process] = kernel process
```
### KILL
```diff
kill "PID"# sends stop message to process
+ -9 #force quit #options from 0-9
```
### KILLALL
```diff
killall "programmname"
```
### TOP
```diff
top #interactive processes (sorted by usage of system resources)
```
### PSTREE
```diff
pstree #shows a tree of Processes(Parent and Subprocesses)
```
### Shebang line (set interpreter)
```bash
#!/bin/python3
```
### CHMOD (Change permissions)
rwx _ _ _  _ _ _
```bash
chmod u+rwx
chmod u+x
```
```bash
chmod g+rwx
```
```bash
chmod o+rwx
```
```diff
- don´t chmod 777 (rxw rxw rxw)
7 = permission to read write and execute
```
### MAN (information about a command)
```bash
man
```
### APROPOS (searchs commands related to a keyword)
```bash
apropos [OPTIONS] keyword
```
### Parse command output to file
```bash
cat file > outputfile #parse only command output(No Errors) to outputfile
cat file &> outputfile #parse output and Errors to outputfile
cat file 2> outputfile #parse only Errors to outputfile
cat file >> outputfile #if outputfile exists than the new file output will append to existing file 
```
### pipe
```bash
ps -ef | grep xeyes # "|" pipes output from "ps -ef" to "grep xeyes"  
```
### FREE (shows free space)
```bash
free
```
### df (shows Hardrives)
```bash
df
```
### uname (system information)
```bash
uname -a #shows system and version of system
```
## Wildcards
### overview
```diff
* 
?
[]
```
### Usage:
List all files that contains "test" in filename
```bash
Ls | grep *test*
```
List all file that contains a number between [0-9]
```bash
Ls | Grep *[0-9]*
```
```bash
ls te?t 
```
## Priorities (Not complete)
```bash
nice 
```
## enviroment Variabels
```bash
- PATH
```
Usage:
```bash
printenv #shows all variables
echo $PATH #outputs a Variable
```

## Subprocesses
```bash
./datei.sh &
```
or if process is aready running
```bash
ctr+z
```
return to subprocess 
```bash
bg # background
fg #foreground
```

## VI
```diff
- vimtutor
```
## Makefiles
```diff
- anschauen!
```
## important files
