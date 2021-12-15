
**Powerpoint 1**
**Desktop Environment** 
* Windows and macOS are very limited to just a single GUI/DE whereas in Linux, there are multiple choices
* Linux contains a file manager to conduct file maitenence, a favorites bar, launcher, panels that are on the top of the main menu, etc etc.
* Mostly other desktop environments contain a similar yet differen structure varying if has GNOME elements in it or not

**Powerpoint 2**
**What is a shell**
* CLI (Command-Line Interface): its used to interact with a computer program through the uses of commands to send to the program within lines of text
* The console terminal holds virtual consoles that are within the Linux system, they can be accessed by using a keyboard and mouse and a user ID and password
  * It would use BASH as the default shell 

* Terminal Emulator: a program that allows the access to the Linux CLI
* This application would be called "Terminal"
  
*The Bash Shell*
* a program that provides interactive access to Linux
* Bash Shortcuts
  * Ctrl + A - takes you to the start of the command line
  * Ctrl + E - takes you to the end of the command line
  * Ctrl + K - delete from curser at the end
  * Ctrl + U - delete from cursor at beginning
  * Ctrl + W - delete from start of word
  * Ctrl + Y -paste word or text after cursor
  * Ctrl + XX - move between command line and cursor position
  * Alt + B - move back a word
  * Alt + F - move forward a word
  * Alt + D - delete end of word startung at cursor
  * Alt + C - capitalize end of word starting at cursor
  * Alt + U - make uppercase
  * Alt + I - make lowercase
  * Alt + T - swap current word to previous word
  * Ctrl + F - move forward a character
  * Ctrl + B - move backa character
  * Ctrl + D - delete character
  * Ctrl + H - delete character before cursor
  * Ctrl + T - change character with previous
  * Ctrl + R - search history backwards
  * Ctrl + G - exit history search mode
  * Ctrl + P - goes to previous command in history search 
  * Ctrl + N - goes to next command in history search
  * Alt + . - last word of previous command
  * Ctrl + L - clear screen
  * Ctrl + S - stops output
  * Ctrl + Q - shows output 
  * Ctrl + C _ terminates comand
  * Ctrl + Z - suspends terminal
  * !! - run last command 
  * !blah - will run recent command that starts with word after !
  * !blah:p - prints out command that word after ! would run
  * !$ - last word of previous command
  * !$:p - subsitute word after !
  * !* - previous command except last word
  * !*:p - prints what !* would substitute

CTRL + Shift + C = copy
CTRL + Shift + V = paste

*Shell Prompt*
* if a $ isnt shown but a # is, you are signed in with sudo privileges


Basic Command Usage
* date - displays date + time
* cal - calendar 
* df - displays current amount of remaining space in disk drives
* free
* displays free memory left
* uname - displays information about system
* clear - clears screen
  
by using left and right commands you can acess previous commands.

**Powerpoint 3**
**How to navigate the Filesystem**
* The file system in linux is bult through a hierarchial directory structure like a tree 
* directory = folder
* / is the root of the system
  
*Navigating the FS in the CLI*
* everything in the file system


![Command](:commands.png)

*Commands to use*
* pwd command - used to display current working directory
* cd command - changing directories
* using ../ will put you in the previous directory
* . = current directory


  * cd + destination - can move around from the directories
  * cd, cd ~, and cd $HOME all go back to the home directory
  * cd - : goes back to the previous directory

/home/$USER/Downloads is an absolute path

* ls command - listing files in a directory
  * man ls will show what options can be used with the ls command
    * ls -a lists all files in working Directory + hidden files
    * ls -a ~/Pictures: all files inside directory
    * ls -lR ~/Pictures: long list of files inside recursively
  * ls -t ~/Documents - lists by last motified
  * ls - S ~/Documents - lists by file size
  * ls -X ~/Documents - lists by extension
  * ls - r ~/Documents lists files in reverse
  * ls - R ~/Documents - lists files recursively
  * ls --help - lists every option for ls

Types of pathnames:
* Absolute Path - the full pathname starting at the root, ex: 
  * /home/john/Downloads/song.mp3

* Relative Path - specific and short pathname from the current directory
  * ex: Downloads/song.mp3



