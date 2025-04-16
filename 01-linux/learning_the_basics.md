# Today we are going to learn the basic commands and using Terminal.

## 1. Getting to Know the Terminal 🖥️

Terminal = the Command Line Interface (CLI)

  In Linux, the terminal is where all the magic happens. It’s your command center to interact with the system. You type commands to run programs, move files around, or even install software. It might look intimidating at first, but trust me, it’s powerful once you get used to it! 😏

### Basic Commands to Get Started

  `pwd` — Print Working Directory (shows where you currently are in the file system)

  `ls` — List files and directories in the current directory

  `cd <directory>` — Change Directory (move between directories)

  `mkdir <folder_name>` — Make a new directory/folder

  `rmdir <folder_name>` — Remove a directory (it’s gotta be empty tho!)

  `echo <text>` — Display a string of text in the terminal

  `clear` — Clears the terminal screen (gets rid of all the clutter)

Example:

    $ pwd
    /home/user
    $ ls
    Documents  Downloads  Pictures
    $ cd Documents
    $ mkdir NewFolder
  
## 2. File Management 🔥

Linux is all about files and folders, and Kali is no different. Here's how to handle them:

   `cp <source> <destination>` — Copy files/folders

   `mv <source> <destination>` — Move files/folders (you can also use it to rename files)

   `rm <file>` — Remove (delete) files

   `rm -r <folder>` — Remove a directory and all its contents

   `cat <file>` — View the contents of a file in the terminal

   `nano <file>` — Open a file in a text editor (nano is simple and user-friendly)

Example:

    $ cp file.txt /home/user/Documents/
    $ mv old_name.txt new_name.txt
    $ rm oldfile.txt
    $ nano textfile.txt

## 3. Package Management 📦

Kali Linux is a Debian-based distro, so it uses APT (Advanced Package Tool) to manage software.

   `sudo apt update` — Updates the list of available packages

   `sudo apt upgrade` — Upgrades all the packages that need updating

   `sudo apt install <package_name>` — Installs a package

   `sudo apt remove <package_name>` — Removes an installed package

   `sudo apt search <package_name>` — Searches for a package in the APT repository

Example:

    $ sudo apt update
    $ sudo apt upgrade
    $ sudo apt install nmap
    $ sudo apt remove firefox

## 4. User Management 👤

In Linux, you work with users and groups. Here's how you manage them:

   `whoami` — Shows the current user

   `id <username>` — Displays information about a user

   `sudo adduser <username>` — Adds a new user

   `sudo deluser <username>` — Deletes a user

   `sudo passwd <username>` — Change the password for a user

   `sudo usermod -aG <group_name> <username>` — Adds a user to a group

Example:

    $ whoami
    user
    $ sudo adduser newuser
    $ sudo passwd newuser

## 5. Permissions in Linux 🔐

Linux is all about file permissions. You'll often need to control who can read, write, and execute files.

   `r` — Read permission (view the contents of a file)

   `w` — Write permission (edit the contents of a file)

   `x` — Execute permission (run a file or program)

   `chmod <permissions> <file>` — Change the permissions of a file

Example:

    $ chmod +x script.sh
    $ ls -l script.sh

## 6. Networking (Important for Kali) 🌐

Kali is mostly used for network security and penetration testing. So, networking commands are key!

   `ifconfig` — Shows your network interfaces

   `ping <address>` — Ping an IP address (check if it’s reachable)

   `netstat` — Displays network connections and routing tables

   `ip a` — Another way to view network interfaces

   `nmap <target>` — Scan a network for open ports (very useful in Kali!)

Example:

    $ ifconfig
    $ ping google.com
    $ nmap 192.168.1.1

## 7. Process Management ⚙️

Linux runs a lot of background tasks (called processes). Here's how to manage them:

   `ps` — Shows a list of running processes

   `top` — Displays a dynamic list of processes

   `kill <pid>` — Kills a process by its process ID (PID)

   `killall <process_name>` — Kills all instances of a process

   `bg` — Resumes a paused process in the background

   `fg` — Brings a background process to the foreground

Example:

    $ ps aux
    $ top
    $ kill 1234
    $ killall firefox

## 8. Kali Linux Tools 🔧

Since you're using Kali, you're probably interested in the security tools it comes with. Here are some essentials:

  `nmap` — Network scanner (use to discover hosts and open ports)

  `metasploit` — Penetration testing framework (use for testing exploits)

  `airmon-ng` — Wireless network monitoring tool (useful for WiFi testing)

  `burpsuite` — Web vulnerability scanner and proxy tool

## 9. Shortcuts and Fun Stuff 🖱️🎮

   `Ctrl` + `Alt` + `T` — Open a new terminal window

   `Ctrl` + `C` — Stop a running command

   `Ctrl` + `D` — Exit the terminal

   `Tab` — Auto-completes commands and file names (saves tons of time)

  `Shift` + `Page Up`/`Page Down` — Scroll through terminal history
