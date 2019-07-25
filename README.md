This repository contains all of my works of CSE324(**Operating System Lab** ) course.

## Scheduling Algorithms
To decide which process to execute first and which process to execute last to achieve maximum CPU utilisation, computer scientists have defined some algorithms, they are:

- <td> <a href="https://github.com/rabbycse/Operating-System/tree/master/sources/01/First%20Come%20First%20Serve">First Come First Serve(FCFS) Scheduling</a>
- <a href="https://github.com/rabbycse/Operating-System/tree/master/sources/02/Shortest%20Job%20First">Shortest-Job-First(SJF) Scheduling</a>
- <a href="https://github.com/rabbycse/Operating-System/tree/master/sources/03/Priority%20Scheduling">Priority Scheduling</a>
- <a href="https://github.com/rabbycse/Operating-System/tree/master/sources/04/Round%20Robin(RR)%20Scheduling">Round Robin(RR) Scheduling</a>
- <a href="https://github.com/rabbycse/Operating-System">Multilevel Queue Scheduling</a>
- <a href="https://github.com/rabbycse/Operating-System">Multilevel Feedback Queue Scheduling</a></td>

<br></br>

## Useful Linux Commands

Linux commands
```
cat [filename]	                        # Display file’s contents to the standard output device (usually your monitor).
cd /directorypath                       # Change to directory.
chmod [options] mode filename           # Change a file’s permissions.
chown [options] filename	        # Change who owns a file.
clear	                                # Clear a command line screen/window for a fresh start.
cp [options] source destination         # Copy files and directories.
date [options]	                        # Display or set the system date and time.
df [options]	                        # Display used and available disk space.
du [options]	                        # Show how much space each file takes up.
file [options] filename	                # Determine what type of data is within a file.
find [pathname] [expression]	        # Search for files matching a provided pattern.
grep [options] pattern [filesname]	# Search files or output for a particular pattern.
kill [options] pid	                # Stop a process. If the process refuses to stop, use kill -9 pid.
less [options] [filename]	        # View the contents of a file one page at a time.
ln [options] source [destination]	# Create a shortcut.
locate filename	                        # Search a copy of your filesystem for the specified filename.
lpr [options]	                        # Send a print job.
ls [options]	                        # List directory contents.
man [command]	                        # Display the help information for the specified command.
mkdir [options] directory	        # Create a new directory.
mv [options] source destination	        # Rename or move file(s) or directories.
passwd [name [password]]	        # Change the password or allow (for the system administrator) to change any password.
ps [options]	                        # Display a snapshot of the currently running processes.
pwd	                                # Display the pathname for the current directory.
rm [options] directory	                # Remove (delete) file(s) and/or directories.
rm -rf directory:                       # Delete non-empty directories
rmdir [options] directory	        # Delete empty directories.
ssh [options] user@machine	        # Remotely log in to another Linux machine, over the network. Leave an ssh session by typing exit.
su [options] [user [arguments]]	        # Switch to another user account.
tail [options] [filename]	        # Display the last n lines of a file (the default is 10).
tar [options] filename	                # Store and extract files from a tarfile (.tar) or tarball (.tar.gz or .tgz).
top	                                # Displays the resources being used on your system. Press q to exit.
touch filename	                        # Create an empty file with the specified name.
who [options]	                        # Display who is logged on.
```



#### Some basic bash snippets I use to introduce shell scripting to my Linux class.
```
#!/bin/bash

# viewing environment variables
echo "The value of the home variable is: "
echo $HOME

# issue a command
echo "The output of the pwd command is: "
pwd

# that's boring, grab output and make it readable
echo "The value of the pwd command is $(pwd)"

# assign command output to a variable
output=$(pwd)
echo "The value of the output variable is ${output}"

# view data on the command line
echo "I saw $@ on the command line"

# read data from the user
echo "Enter a value: "
read userInput
echo "You just entered $userInput"

# concatenate userinput with command output
echo "Enter a file extension: "
read ext
touch "yourfile.${ext}"

# check to see if a file exists
if [ -d /etc/sysconfig ]; then
        echo "That file is there and a directory"
else
        echo "Not there or not a directory"
fi
```

