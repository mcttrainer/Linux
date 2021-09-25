# Package Management

Package is nothing about a software that can be installed on a GNU/Linux Operating System.

Each family has a different mechanism for managing pacakges 


Debian - dpkg -- apt
RedHat - rpm  -- yum
Suse   - Yast
Slackware 
Arch.   - pacman


How can a Package Installed in Linux?

3 ways

1. From Repositories
2. Downloading the binary (executable)
3. Compiling(build) and installing

Package repository is a  central location where your distribution maintainer keeps all the packages available for you.

firefox
git
vim
tree
disk utilities

How does my linux os know where to download packages from?

sources --> /etc/apt


Debian 
`sudo apt-get update`
 Synchronizes the indexes with your distribution repositories

`sudo apt-get upgrade`
Upgrades all the existing packages

`sudo apt-get install <packageName>`
    Installs <packageName> 

`sudo apt-get remove <packageName>`
    Removes <packageName> from the system

`sudo apt-get purge <packageName>`
    Removes <packageName> from the system and also deletes any configuration files

`sudo apt auto-remove`
  To remove dependencies or packages that are no longer needed.

How to find list of all packages?

`sudo dpkg --list`
Lists the available packages 
`sudo dpkg --get-selections`
gives the list of installed packages

If a package is not available through the repositories, the binary can be downloaded and installed using dpkg command

`sudo dpkg -i <package>`

The packages that are to be installed on Debian family have .deb extension
very rarely you may see .tar .gz extension


Redhat

Redhat family of operating systems uses rpm as the backend and yum as the frontend for package manangent.
rpm - Redhat Package Manager
yum - Yellowdog Update Manager.

Installing a package:
`sudo yum install <packagename>`



Remove a Package:
`sudo yum remove <packagename>`


rpm is the command to install binaries and list installed packages

`sudo rpm -i <packagename>`

`sudo rpm -qa`
Lists all the installed packafes

`sudo rpm -q <packagename>`
Gives details about the <packagename>
    

    apache2 on Ubunut
    httpd   on Centos
    tree 


Redhat packages are typically have the extension of .rpm





























