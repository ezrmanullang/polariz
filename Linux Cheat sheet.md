
<h3>Bash Commands</h3>
<p>
<b>uname -a</b>
Show system and kernel
</p>
<p>
<b>head -n1 /etc/issue</b>
Show distri­bution
</p>
<p>
<b>mount</b>
Show mounted filesy­stems
</p>
<p>
<b>date</b>
Show system date
</p>
<p>
<b>uptime</b>
Show uptime
</p>
<p>
<b>whoami</b>
Show your username
</p>
<p>
<b>man command</b>
Show manual for command
</p>


<h3>Bash Shortcuts</h3>
<p>
CTRL-c
Stop current command
</p>
<p>
CTRL-z
Sleep program
</p>
<p>
CTRL-a
Go to start of line
</p>
<p>
CTRL-e
Go to end of line
</p>
<p>
CTRL-u
Cut from start of line
</p>
<p>
CTRL-k
Cut to end of line
</p>
<p>
CTRL-r
Search history
</p>
<p>
!!
Repeat last command
</p>
<p>
!abc
Run last command starting with abc
</p>
<p>
!abc:p
Print last command starting with abc
</p>
<p>
!$
Last argument of previous command
</p>
<p>
ALT-.
Last argument of previous command
</p>
<p>
!*
All arguments of previous command
</p>
<p>
^abc^123
Run previous command, replacing abc with 123
</p>


Bash Variables
env
Show enviro­nment variables
echo $NAME
Output value of $NAME variable
export NAME=value
Set $NAME to value
$PATH
Executable search path
$HOME
Home directory
$SHELL
Current shell


IO Redire­ction
cmd < file
Input of cmd from file
cmd1 <(cmd2)
Output of cmd2 as file input to cmd1
cmd > file
Standard output (stdout) of cmd to file
cmd > /dev/null
Discard stdout of cmd
cmd >> file
Append stdout to file
cmd 2> file
Error output (stderr) of cmd to file
cmd 1>&2
stdout to same place as stderr
cmd 2>&1
stderr to same place as stdout
cmd &> file
Every output of cmd to file
cmd refers to a command.


Pipes
cmd1 | cmd2
stdout of cmd1 to cmd2
cmd1 |& cmd2
stderr of cmd1 to cmd2


Command Lists
cmd1 ; cmd2
Run cmd1 then cmd2
cmd1 && cmd2
Run cmd2 if cmd1 is successful
cmd1 || cmd2
Run cmd2 if cmd1 is not successful
cmd &
Run cmd in a subshell
 	
 	
Directory Operations
pwd
Show current directory
mkdir dir
Make directory dir
cd dir
Change directory to dir
cd ..
Go up a directory
ls
List files


ls Options
-a
Show all (including hidden)
-R
Recursive list
-r
Reverse order
-t
Sort by last modified
-S
Sort by file size
-l
Long listing format
-1
One file per line
-m
Comma-­sep­arated output
-Q
Quoted output


Search Files
grep pattern files
Search for pattern in files
grep -i
Case insens­itive search
grep -r
Recursive search
grep -v
Inverted search
grep -o
Show matched part of file only
find /dir/ -name name*
Find files starting with name in dir
find /dir/ -user name
Find files owned by name in dir
find /dir/ -mmin num
Find files modifed less than num minutes ago in dir
whereis command
Find binary / source / manual for command
locate file
Find file (quick search of system index)


File Operations
touch file1
Create file1
cat file1 file2
Concat­enate files and output
less file1
View and paginate file1
file file1
Get type of file1
cp file1 file2
Copy file1 to file2
mv file1 file2
Move file1 to file2
rm file1
Delete file1
head file1
Show first 10 lines of file1
tail file1
Show last 10 lines of file1
tail -F file1
Output last lines of file1 as it changes


Watch a Command
watch -n 5 'ntpq -p'
Issue the 'ntpq -p' command every 5 seconds and display output


Process Management
ps
Show snapshot of processes
top
Show real time processes
kill pid
Kill process with id pid
pkill name
Kill process with name name
killall name
Kill all processes with names beginning name
 	
Nano Shortcuts
Files
Ctrl-R
Read file
Ctrl-O
Save file
Ctrl-X
Close file
Cut and Paste
ALT-A
Start marking text
CTRL-K
Cut marked text or line
CTRL-U
Paste text
Navigate File
ALT-/
End of file
CTRL-A
Beginning of line
CTRL-E
End of line
CTRL-C
Show line number
CTRL-_
Go to line number
Search File
CTRL-W
Find
ALT-W
Find next
CTRL-\
Search and replace
More nano info at:
http:/­/ww­w.n­ano­-ed­ito­r.o­rg/­doc­s.php


Screen Shortcuts
screen
Start a screen session.
screen -r
Resume a screen session.
screen -list
Show your current screen sessions.
CTRL-A
Activate commands for screen.
CTRL-A c
Create a new instance of terminal.
CTRL-A n
Go to the next instance of terminal.
CTRL-A p
Go to the previous instance of terminal.
CTRL-A "
Show current instances of terminals.
CTRL-A A
Rename the current instance.
More screen info at:
http:/­/ww­w.g­nu.o­rg­/so­ftw­are­/sc­reen/


File Permis­sions
chmod 775 file
Change mode of file to 775
chmod -R 600 folder
Recurs­ively chmod folder to 600
chown user:group file
Change file owner to user and group to group


File Permission Numbers
First digit is owner permis­sion, second is group and third is everyone.
Calculate permission digits by adding numbers below.
4
read (r)
2
write (w)
1
execute (x)
