##### Check your Current Location

```bash
pwd
```

##### Current user logged in

```bash
whoami
```

##### Current time/date/timezone all thing

```bash
date
```

##### To check only date

```bash
date +%D
```

##### To check only time

```bash
date +%T
```

##### To check time in the format of H:Min

```bash
date +%H:%M
```
##### List files & directory in long format

```bash
ls -lt
```
##### List files & directories in reverse means (latest wala neeche hoga)

```bash
ls -ltr
```
##### To List the size in human readable format then use this

```bash
ls -lh
```

##### Display Long text file & Search for a word
```bash
less <file>
```

	To go to the last line : `Shift + G`

	 To go to the first line : `P`

- To search from Bottom to top then use : `/` ? "word"
##### To view Content of a file page by page

```bash
more <file>
```

##### To delete directory

```bash
rmdir <dir_name>
```

##### To move back multiple folders at one time

```bash
cd ../../../../
```

##### Make a copy of a file

```bash
cp mini.csv mini_copy.csv
```

##### Read or display top 5 lines from a file

```bash
head -5 <file>
```

##### Read or display top 5 lines from a file from bottom

```bash
tail -n <file>
```

##### Sort the content from a file

```bash
sort <file>
```

##### Sort in reverse order

```bash
sort -r <file>
```

##### Display unique content from file (Means duplicate ignore karo)

```bash
sort <file> | uniq
```

##### A file has 9 lines , split this file in 3 different files

```bash
split -l 3 file
```

##### Search a word and display matching content from a file

```bash
grep "word" <file>
```

##### Search multiple words & display matching content from a file

```bash
egrep "word1"| "word2" <file>
```

##### Perfect Use of Wild Cards

```bash
ls file*.sh or ls file*.py
```

##### Make more than one files at ones

```bash
touch file{1..10}
```

##### Shuffle content of file

```bash
shuf <file>
```

##### Count no of lines in the file

```bash
wc -l file
```

##### Check if two files are identical or not

```bash
cmp fileA fileB
```

##### Compare and display difference between two lines

```bash
diff -u fileA fileB
```

##### Find a file

```bash
find /path -name <file>
```

##### Find a file using "locate"

```bash
sudo updatedb
```

***We Need to update database as the locate command checks the cache and find the file

```bash
locate <file>
```

##### Search specific cmd used in history using grep

```bash
history | grep "cmd"
```

##### Check syntax & options available for a command

```bash
ls --help | more
```

##### Check which executable is using for a cmd

```bash
which zsh
```

##### Use Calculator

```bash
bc
```

##### Check calendar of current year

```bash
cal
```

##### Check how long the linux machine has been running

```bash
uptime
```

##### Record your activity on terminal in a file so that you can see what you did

```bash
script
```

*After done* Press <kbd>Ctrl</kbd> + <kbd>D</kbd> to end

##### Create a Shortcut of a Long command

```bash
alias l="ls -ltr"
```

##### To see the list of shortcut made by alias

```bash
alias -p
```

##### Compress a file in linux

```bash
gzip -k <file>
```

##### Decompress a file in linux

```bash
gzip -d <file>
```

<center>OR</center>

```bash
gunzip <file>
```

##### Compress a folder in Linux

```bash
tar -czf <setFileName.tar.gz> <folder>
```
##### Decompress a folder in Linux

```bash
tar -xzf <file.tar.gz>
```

##### Compress multiple files in one zipped file in Linux

```bash
zip myFiles.zip file1 file2
```

##### List files in zipped file

```bash
unzip -l myFiles.zip
```

##### Decompress the zip file

```bash
unzip myFiles.zip
```

##### Set custom file name while downloading the file from internet

```bash
wget -O "file_name" URL
```

##### How to Call an API on Linux terminal

```bash
curl https://numbersapi.com/random
```

##### Check if an application is installed or not on linux

```bash
rpm -qa | grep app
```

<center>OR</center>
```bash
dnf list installed
```

##### How to list available packages to install on Linux

```bash
apt search <package_name>
```

##### List all Services on Linux

```bash
systemctl list-units --type=service -all
```

##### List all existing Environment variables on Linux

```bash
printenv
```

##### How to ADD a new Environment variables on linux

```bash
export JAVA_HOME="usr/lib/jvm/java"
```

- ***To your current shell like "~/.bashrc" or "~/.zshrc"

##### Print a specfic column from a CSV file

```bash
awk -F ,'{print $2}' file.csv
```

##### Display starting two characters of all line

``
```bash
cut -c1-2 file.txt
```

##### Display a specfic line from a file

```bash
sed -n 'sp' file.txt
```

##### Replace a Specific word within a file

```bash
sed 's/<oldWord>/<newWord>/g' file.txt
```

***This Changes are not permanent

##### Convert the content to Uppercase or Lowercase within a file

```bash
tr [:lower:] [:Upper:] < file.txt
```

```bash
tr [:punct:] z < file.txt
```

```bash
tr [:digit:] z < file.txt
```

##### To delete something (some character)

```bash
tr -d "%d" < test.txt
```

##### To replace the character

```bash
tr "%" "&" < test.txt
```

##### How to extend or shrink size of a file

```bash
truncate -s 100M file.txt
```

***If the file is 1 MB if we extend to 100 MB rest of them are filled with extra machine code***

##### Display following line in vertical in vertical line

```bash
echo "ABCDE" | fold -1
```

##### Change user or Login as different user in Linux

```bash
su <username>
```

***Login as Root user***

```bash
su -
```

##### Modify permissions of a file

```bash
chmod a+rwx <file>
```

*+* Means Add Permissions
*-* Means Remove Permissions


<img width="3904" height="1836" alt="image" src="https://github.com/user-attachments/assets/1faa8ddb-3d56-42a2-a831-f5c758a3a98b" />


##### If you want to check the files

```bash
ls -l <file>
```

##### Change ownership of a file

```bash
chown root <file>
```

***Here root is the placeholder of user

##### Change group ownership of a file

```bash
chgrp <user(paul)> <file>
```

##### Check free RAM Space

```bash
free
```

***Read in human readable format***

```bash
free -h
```

*Total*

```bash
free -th
```

##### Check % Memory & CPU Utilization

```bash
top or htop
```

##### Check disk utilization by some folder

```bash
du -h <folder>
```

##### Check File system available & disk space allocated

```bash
df
```

##### Check CPU/Core/thread info of your linux machine

```bash
lscpu
```

##### Check type of architecture of your linux machine

```bash
arch
```

***This works on fedora as i have tested on it the cmd which works on all linux distro***

```bash
uname -m
```

##### Check OS name of Linux machine

```bash
uname -a
```

<center>OR</center>

```bash
cat /etc/os-release
```

##### Check if a process is running or not

```bash
ps -ef | grep java
```

##### Get PID of a process

```bash
pgrep chron
```

##### Stop a process by PID

```bash
kill -9 PID
```

##### Stop a process by it's name

```bash
pkill <name>
```

##### See all the active jobs

```bash
jobs
```

##### Resume a job in background

```bash
bg
```

##### Resume a job in foreground

```bash
fg
```

##### Run a script in background

```bash
nohup ./script >/dev/null &
```

##### Check if a IP : Port is accessible and open or not

```bash
telnet IP Port
```

##### Check if port is open or not our server

```bash
netstat -putan | grep 80
```

##### Check all hubs in network path to reach a website

```bash
traceroute <website>
```

##### Create a new user on linux

```bash
useradd <username>
```

***Check if user is created or not***

```bash
id <username>
```

##### Create a new user group on our linux

```bash
groupadd <name>
```

##### See if group is created or not

```bash
cat /etc/group
```

##### Check user ID or Group ID of a user

```bash
id <user>
```

##### Delete a user or group

```bash
userdel <user>
```

```bash
groupdel <group>
```

##### Change the group of a user

```bash
usermod -G <group_name> <User>
```

##### Give Permission at ones of same extension at ones

```bash
chmod +x *.sh
```


