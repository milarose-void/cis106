**Handling Text Files** 
*Cat* 
* the cat command is used for displaying content of the file
* Cat = concatenate


cat /etc/passwd = display content of file

cat /etc/passwd -n = numbers all the users that are in the system

man cat = learning more about what the cat command does

cat /etc/passwd -e = lets the user know when the code ends

 *Tac* 

* the ability to use the command but in reverse

*More*
* a pager program used to lists content of the text, one page at a time
  * less is the opostie of what more is
  * less /etc/password will prompt you to open the password

*Head* 

head /etc/passwd = first 10 lines 

man head = lists information about the head command

head /etc/passwd/ -() = any number of choice can show what lines 

nano = text editor used within the command 
name = input("hi, what's your name?)
ctrl + O = save

chmod u+x cis106.py = 

python3 cis106.py = 

head cis106.py =

*Tail* 

* tail = contains last N number of lines of a given file

tail [-1]

*Cut*
* extracts a specific section of each line of a file and displays it on the screen 
  
cut -d ' ' -f 1,3 = cuts out sections between 

cut -d ':' -f1,7 /etc/passwd = only outputs the lines with the 1 and 7 fields

cut -d ':' -f1,7 --output-delimiter=' =  ' /etc/passwd | tail -1 = 

*Paste* 
* merge 2 files together

nano ip.txt (1.1.1.1)
nano user (bob.potato)

paste ip.txt user.txt

*Sort* 
* sorting data
  * alphabetically
  * reverse order
  * by number
  * by month

sort -o userSorted.txt users.txt = sorts file by user
sort -r users.txt = sorts in reverse
sort -n phoneNumbers.txt (numeric order)
sort -c usersSorted.txt = checks if files are sorted
sort -u users.txt = sort and remove duplicate entries

*Wc*
* printing the number of lines 

wc -l /etc/passwd = lines in a command

wc -c users.txt = displays number of bytes in a file 

*Tr*
* translates or deletes characters from a standard output

cat /etc/passwd | tr "." "," 

*Diff*
* used only if one file is different from another

*Grep* 
* used to match a string pattern from a file or standard output when using the pipe
grep 'linux' linux.txt = finds how many times that specific word was used 
grep -option "word or phrase" filename 

grep -i 'linux' linux.txt = both upper and lower case

cat -n linux.txt | grep -1 "linux"

grep (command to match a pattern) -in (options turn case sensisitvity off + line number it's on) "linux" (word phrase to look for) ~/linux.txt (location)

grep "/bin/bash" /etc/passwd

ip addr | grep "inet" = showing the line that finds the ip address line

ip addr | grep "inet" | head -3 = shows the first 3 lines

ip addr | grep "inet" | tail -1 = shows the last line

Rev
* reverses characters in a file 
rev file

STDOUT = standard output (monitor) 1
STDIN = standard input (keyboard) 0
STDERR = standard error  2

ip addr >ipaddresses.txt  =redirecting files that are outputted to be saved somewhere else 

2>ipaddresses.txt

ls Downloads/ documents/ > listfiles.txt 2>errorlog.txt = redirecting correct file to where it's supposed to be and another with the error into the errorlog.txt

ls Downloads/ >myfiles.txt > myfiles.txt 2>myfileserror.txt

>>myfiles.txt = allows file to be transferred and not be overwritten

ls Downloads/ bad/ > log.txt &> log.txt = error and output are both saved into the files

* with the cat command it will copy standard outputs and then it can be redirected to create a file

the "|" allows to redirect standard output to a standard input
* man  ls | grep "human-readable" = use grep to look for a string in a particular man page
  

Alias
alias name_of_alias="command here"
alias add = git add


