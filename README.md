# Ubuntu-Linux-Distro-Cheat-Sheet

![enter image description here](https://raw.githubusercontent.com/theanasuddin/Ubuntu-Linux-Distro-Cheat-Sheet/main/cover.png)

## Install Ubuntu Desktop :computer:
### Recommended System🖥 Requirements :memo::
 - 2 GHz dual core processor or better
 - 4 GB RAM (system memory)
 - 25 GB of free hard drive space
 - VGA capable of 1024x768 screen resolution
 - Internet access is helpful
 - Either a DVD drive or a USB port for the installer media

### Download :arrow_down: Ubuntu:
> :pushpin: It's better to ownload the latest LTS version of Ubuntu, for desktop PCs and laptops. LTS stands for long-term support — which means five years of free security and maintenance updates, guaranteed.

Click ***[here](https://ubuntu.com/download/desktop)*** to download latest Ubuntu Desktop 🖥 ISO image file from Ubuntu website.

### Make Bootable USB :floppy_disk::
> :pushpin: Format the USB flash drive in FAT32 mode. Download Rufus to create a bootable USB drive from the downloaded .iso image file. Rufus is a free and open-source portable application for Microsoft Windows that can be used to format and create bootable USB flash drives or Live USBs. You may use other tools like Etcher, UNetbootin to do this.

Click ***[here](https://rufus.ie/)*** to download Rufus.

## Useful Commands 
### Update Ubuntu:
Sync the package index files from their sources:

    $ sudo apt-get update
    or
    $ sudo apt update

Install the newest versions of all installed packages:

    $ sudo apt-get upgrade
    or
    $ sudo apt upgrade

To reboot the system after updating (if needed):

    $ sudo reboot

## GNOME Desktop Environment
### GNOME:
> :pushpin: ***[GNOME](https://www.gnome.org/)*** is a free and open-source desktop environment for Unix-like operating systems. Latest Ubuntu releases use GNOME desktop environment by default. 

### GNOME Shell:
> :pushpin: GNOME Shell provides core user interface functions for GNOME, like switching to windows and launching applications. User interface elements provided by GNOME Shell include the Panel at the top of the screen, the Activities Overview, and Message Tray at the bottom of the screen. 

### GNOME Shell Extensions:
> :pushpin: GNOME Shell extensions are small pieces of code written by third party developers that modify the way GNOME works. (If you are familiar with Chrome Extensions or Firefox Addons, GNOME Shell extensions are similar to them.) You can find and install GNOME Shell extensions using ***[this](https://extensions.gnome.org/)*** website.

Install GNOME shell extension package:

    $ sudo apt install gnome-shell-extensions

### Install GNOME Tweaks:
To customize your desktop further, you may install GNOME Tweaks. You can get it from Ubuntu Software or run the following command:

    $ sudo apt install gnome-tweaks

## Install S/W, Software Management 
Softwares and packages can be downloaded from various sources and in various ways. Popular ways for installing packages are:

 - Ubuntu Software
 - [*Snap*](https://snapcraft.io/)
 - Synaptic Package Manager
 - [*Ubuntu Packages*](https://packages.ubuntu.com/)
 - Download directly from specific website etc.

### Install Synaptic Package :package: Manager:
> :pushpin: Synaptic is a graphical package management program for apt. It provides the same features as the apt-get command line utility with a GUI front-end based on Gtk+.

Install using:

    $ sudo apt-get install synaptic

### APT:
> :pushpin: The apt command is a powerful command-line tool, which works with Ubuntu’s _Advanced Packaging Tool_ (APT) performing such functions as installation of new software packages, upgrade of existing software packages, updating of the package list index, and even upgrading the entire Ubuntu system.

Installation of packages using the apt tool is quite simple. For example, to install a package, type the following:

    $ sudo apt install SOFTWARE_NAME

Here, SOFTWARE_NAME denotes the name of the package you want to install.

### Commands  To Install Some Useful Softwares & Packages:
 - Chromium
   
       $ sudo snap install chromium
 - Thunderbird
   
       $ sudo snap install thunderbird
 - Visual Studio Code
   
       $ sudo snap install code --classic
 - Eclipse
   
       $ sudo snap install eclipse --classic
 - Apache NetBeans
   
       $ sudo snap install netbeans --classic
 - FileZilla Client
   
       $ sudo apt-get install filezilla
 - GIMP
   
       $ sudo snap install gimp
 - kdenlive
   
       $ sudo snap install kdenlive
 - OBS Studio
   
       $ sudo snap install obs-studio
 - Postman
   
       $ sudo snap install postman
 - Spotify
   
       $ sudo snap install spotify
 - VLC
   
       $ sudo snap install VLC

### Avro Phonetic For Linux:
> :pushpin: GitHub ***[repository](https://github.com/maateen/avro)*** for Avro Phonetic.

  ## Terminal/CLI
  Ubuntu's default terminal is gnome-terminal. Other popular terminal apps are:
 - xterm   
 - rxvt   
 - konsole   
 - terminator

### Terminal Command:
A terminal command can have three parts:
 - Command 
 - Option 
 - Argument

### Essential Terminal Commands:
***FILE*** :file_folder:
Command  | Function
------------- | -------------
cat  | Open a file, Add multiple files, Create new file
tac  | See few ending lines from a file
head  | See first 10 lines from a file
tail  | See few ending lines from a file, by default 10 lines
touch  | Create a new file. Usage: `$ touch \<filename\>`
mv  | Change filename
rm  | Remove file

***DIRECTORY*** :open_file_folder:
Command  | Function
------------- | -------------
pwd  | Present Working Directory. Shows the whole directory path where terminal is at right now
mkdir  | Create new directory. Usage: `$ mkdir \<directoryname\>`
rmdir  | Remove a directory. Usage: `$ rmdir \<directoryname\>`
cd  | Open home directory
cd ~  | Open home directory
cd ..  | Change parent directory
cd -  | Return back to last opened directory
cd ~/Documents  | Jump to Documents directory under home directory
cd /var  | Jump to var directory from root directory (/)
ls  | See all contents of current directory 
ls -a  | See all contents with hidden files of current directory 
tree  | See a tree view of file system
tree -d  | See a tree view only of directories

***FIND*** :mag:
Command  | Function
------------- | -------------
locate  | Used to search files and directories. grep command is also used with locate command to filter more. Usage: `$ locate zip \| grep bin` , this command gives a list of all files and folders containing this two words: zip and bin 
updatedb  | Update database of name listings
find  | This command is used to search for files, it has multiple usage with option and argument
pipe (\|)  | Not a command itself but is used frequently with other commands
sudo  | Abbreviation of "super user do". It allows programs to be executed as a super user (aka. root user) or another user.
man  | See documentation of any command

## Programming In Ubuntu
### C/C++ Programming:
Install C/C++ compiler:

    $ sudo apt-get update
    $ sudo apt-get install build-essential manpages-dev

To check if the compiler is installed properly:

    $ whereis gcc
    $ which gcc
    $ gcc --version

Compile and run c code:

    $ gcc hello.c -o hello
    $ ./hello

Compile and run c++ code:

    $ g++ hello.cpp -o hello
    $ ./hello

### Installing Code::Blocks:
At first, add Code::Blocks repository to ubuntu software list, then update ubuntu package list:

    $ sudo add-apt-repository ppa:damien-moore/codeblocks-stable
    $ sudo apt-update

then install using:

    $ sudo apt install codeblocks

### Java Programming:
Installing the Default JRE/JDK. Execute the following command to install the default Java Runtime Environment (JRE), which will install the JRE from OpenJDK 11:

    $ sudo apt update
    $ sudo apt install default-jre

Verify the installation with:

    $ java -version

You may need the Java Development Kit (JDK) in addition to the JRE in order to compile and run some specific Java-based software. To install the JDK, execute the following command, which will also install the JRE:

    $ sudo apt install default-jdk

Verify that the JDK is installed by checking the version of `javac`, the Java compiler:

    $ javac -version

Compile and run Java code:

    $ javac Hello.java
    $ java Hello

### Install XAMPP:
Download XAMPP from [***Apache Friends***](https://www.apachefriends.org/index.html). Search for "install xampp on ubuntu". Follow some tutorials online and you will be good to go.

### Install Ubuntu Make:
You can use Ubuntu Make to install and update different development tools easily. To install:

    $ snap install --classic ubuntu-make

Use the following command to see a list of Ubuntu Make supported tools and platforms:

    $ umake --list
    $ ubuntu-make.umake

To download Android Studio, use the following command:

    $ umake android
