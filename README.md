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



#### Wine Setup
```
sudo dpkg --add-architecture i386 
sudo add-apt-repository ppa:wine/wine-builds
sudo apt-get update
sudo apt-get install --install-recommends winehq-devel
```

#### Git install
```
sudo apt-get install git
```

#### Install Notepadqq in Ubuntu
```
sudo add-apt-repository ppa:notepadqq-team/notepadqq
sudo apt-get update
sudo apt-get install notepadqq
````
#### Sublime install
```
sudo add-apt-repository ppa:webupd8team/sublime-text-3
sudo apt-get update
sudo apt-get install sublime-text-installer
````

#### Dropbox Headless Install
```
32-bit:
    cd ~ && wget -O - "https://www.dropbox.com/download?plat=lnx.x86" | tar xzf -
64-bit:
    cd ~ && wget -O - "https://www.dropbox.com/download?plat=lnx.x86_64" | tar xzf -
    
    ~/.dropbox-dist/dropboxd
    
    sudo apt install nautilus-dropbox
    
    Start
         dropbox start [-i]
    Auto Start
        dropbox autostart y
```

#### Linux GIMP (Photoshop) install
```
sudo apt-get install gimp 
```

#### Avro install
```
wget "https://github.com/maateen/avro/releases/download/v2.0/avro_2.0-1_all.deb"
 
sudo dpkg -i avro_2.0-1_all.deb
  
sudo apt-get install -fy
  
ibus restart

Keyboard Layout
  ১ System Settings এ গিয়ে Keyboard Layout সিলেক্ট করুন।
  ২ Add Layout বাটন এ ক্লিক করুন (নিচে ছোট + চিহ্ন)
  ৩ Choose a Layout স্ক্রিন এ লিখুন Bengali
  ৪ একটি খুব সহজ Layout হচ্ছে Bengali (Probhat), ওটা সিলেক্ট করে ডাবল ক্লিক করুন।
Tips: সহজে Layout পাল্টানোর জন্য Shift+Caps Lock ব্যবহার করুন।
```

#### Chromium Browser
```
sudo add-apt-repository ppa:canonical-chromium-builds/stage
sudo apt-get update
sudo apt-get install chromium-browser
```

#### Xampp Install
```
For Ubuntu 32 bit :
wget https://www.apachefriends.org/xampp-files/7.0.2/xampp-linux-7.0.2-1-installer.run
sudo chmod +x xampp-linux-7.0.2-1-installer.run
sudo ./xampp-linux-7.0.2-1-installer.run

For Ubuntu 64 bit :
wget https://www.apachefriends.org/xampp-files/7.0.2/xampp-linux-x64-7.0.2-1-installer.run
sudo chmod +x xampp-linux-x64-7.0.2-1-installer.run
sudo ./xampp-linux-x64-7.0.2-1-installer.run

How to Remove:
sudo /opt/lampp/lampp stop
sudo rm -rf /opt/lampp

File permission:
cd /opt/lampp
sudo chmod 777 htdocs
```

#### VLC install
```
sudo apt-get install synaptic vlc
```

#### Bangla Fonts Support
```
sudo apt-get install fonts-beng fonts-beng-extra fonts-lohit-beng-bengali;
apt-cache search bengali
```

#### Web Siter Coper Httrack
```
sudo apt-get install webhttrack
```

#### Weather Check
```
curl wttr.in/your Location

curl wttr.in/brahmanbaria
```

#### Deluge BitTorrent Client Installer
```
sudo apt-get install deluge
```

#### Flash Player install
```
sudo apt-get install firefox ubuntu-restricted-extras

sudo apt-get install ttf-mscorefonts-installer unrar gstreamer0.10-plugins-bad-multiverse libavcodec-extra-53 gstreamer0.10-plugins-ugly gstreamer1.0-plugins-ugly adobe-flashplugin flashplugin-installer gstreamer0.10-plugins-bad gstreamer1.0-plugins-bad gstreamer0.10-ffmpeg gstreamer1.0-libav gstreamer0.10-fluendo-mp3 gstreamer1.0-fluendo-mp3 chromium-codecs-ffmpeg-extra

sudo apt-get install flashplugin-installer
sudo apt-get install adobe-flashplugin
```

#### Color Picker
```
sudo apt-get install gpick
```

#### File Zilla
```
sudo add-apt-repository ppa:adabbas/1stppa
sudo apt-get update
sudo apt-get install filezilla
```

#### Google Drive Install
```
sudo add-apt-repository ppa:nilarimogard/webupd8
sudo apt-get update
sudo apt-get install grive
```


