**Managing Files and Directories**
command -option argument
ls       -l     ~/Downloads

*Creating files and directories*
mkdir command
* make one or multiple directories
* mkdir + name of directory
* can be used with absolute or relative path
  * a directory can use spaces as long as it's between ' ' or " "
  * an error will pop up if name directory exists already
Examples:
* directory with space in name: 
  * mkdir wallpapers/new\ cars
  * mkdir wallpapers/'cities usa'
* create multiple directories:
    * mkdir wallpapers/cars wallpapers/cities wallpapers/forest
* create a directory with a parent directory
  * mkdir -p wallpapers_others/movies

touch command 
* create files 
* create several files
  * touch list_of_cars.txt script.py names.csv

rm command 
* removes files
* rmdir removes empty directories
* rm -r removes non-empty directories. not recommended
* using -i or -I will prompt asking for confirmation before removing file(s)

*Moving and copying files and directories*
mv command
* moves and renames files

mv + source + destination

for files:
mv + file/directory to rename + new name 

* to move a directory from one directory to another using absolute
  * sudo mv ~/Downloads/theme /usr/share/themes
* to move a file from one directory to another combining absolute and relative
  * mv Downloads/english_homework.docx /media/student/flashdrive
* to move multiple directory/files to another directory
  * mv games/ wallpapers/ rockmusic/ /media/student/flashdrive
* to move and rename a file in the same command 
  * mv Downloads/cis106homework.docx Documents/new_cis106homework.docx

cp command
* to copy multiple files into a single command
  * sudo cp -r script.sh program.py home.html assets/ /var/www/html

*Working with links* 
Inode - data structur that contains all info of a file and it is unique
* to find it it is ls -i
* use stat command on a file to display inode data

Hard Links
* files that contain data of the hard drive
* data on any link will not be deleted unless all the links are
* to create a hard link its ln file ~Downloads/fileHL

Soft Links
* it shows other files instead of data in the hard drive
* these are more easier to modify than hard links
* to create a symbolic link its ln -s file fileSL

![screenshot](Screen%20Shot%202021-12-11%20at%207.01.37%20PM.png)

*Using Wildcards* 
* wildcards are used to represent or replace letters in a filename




the "*" can match anything or nothing and is able to match any number of characters
   * benefits when you forget the file name but remember the extension or look for all files that end with the same extension
 * "ls *.txt" will match all files that end with .txt regarless of size or any other factors

the "?" can only match one character
* can be used when looking for hidden files
* to list all hidden files: ls .??*

it is not the same as using * as . is current directory and .. is previous but it can work if its ./.* or ../.* to match files in either current or parent directory

the "[]" wildcard is used to match characters in range
* if an exclamation point is used, it is to exclude whats inside the brackets
* to match all files whose name does not have a number in it 
  * ls *[!0-9].*
* to match all files that beins with a letter from a-p or starts with the letters s or c
  * ls [a-psc]*
* to mach all files whos name begins with an y 3 combination of numbers 
  * ls [0-9][0-9][0-9]$USER

Brace Expansion
* it is not a wildcard but is another feature of bash that allows arbiturary strings to be attached
* ![screenshot example from PPT slide](Screen%20Shot%202021-12-11%20at%207.57.20%20PM.png)

mkdir -p music/{jazz,rock/{mp3files,videos,oggfile}}/new
tree music/

ranger - visual file manager (sudo apt install ranger)
