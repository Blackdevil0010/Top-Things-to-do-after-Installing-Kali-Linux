#Top-Things-to-do-after-Installing-Kali-Linux
_____________________________________________________________________________________________________________________________________________________________________


Installing Guake Terminal
-------------------------
To install Guake Terminal simply go:

in terminal  sudo apt get install guake

Code language: JavaScript (javascript)
Now we also want Guake to start automatically the next time we reboot our system, for that, we enter:

in terminal sudo cp /usr/share/applications/guake.desktop /etc/xdg/autostart/
in terminal sudo reboot now
_____________________________________________________________________________________________________________________________________________________________________

Install your Favorite Code Editor
---------------------------------
Downloading the Visual Studio Code deb package
First, you need to download the VSCode deb package. This automatically installs the Visual Studio Code Apt repository, so we are able to update our Visual Studio 
Code editor.  Choose the 64bit .deb package.

Install Visual Studio Code
First CD into your Downloads folder, or wherever you have downloaded the file to.

in terminal  cd Downloads/

Then we just install it using Apt.

in terminal  sudo apt install ./code_yourversion_amd64.deb

Starting Visual Studio Code
And that’s it. Now you can already go ahead and start VSCode via the app menu.


Geany Code Editor
------------------

Geany is a free, open-source, feature-rich, and highly customizable code editor. It can be used with various programming languages such as Python, HTML5, PHP,
JAVA, JAVAscript, Cin terminal , C++, Ruby, Swift, Bash and many more.

in terminal  sudo apt-get install geany

_____________________________________________________________________________________________________________________________________________________________________


Setting up a VPN
----------------
I have recently written an article where I compare the two most popular VPN Providers out there. I always like to use a VPN when working with any security
distribution. So I always have VPN Setup that automatically connects the VPN once I boot the system. But ideally, you have that set up on your Router.
That ensures that all your Internet traffic is routed through the VPN.

I use NordVPN in this example because that’s what I am currently using myself. I have an affiliation with both NordVPN and PIA, so if you decide to sign up with 
them, use my link and I get a small provision, helping me to pay for server cost. As always, I only recommend stuff that I personally use.

Being a Bug Bounty Hunter, I need to be able to quickly change IPs to avoid bans on websites. NordVPN serves me well as I have set up an alias and just need to 
type “reconnect” and NordVPN automatically reconnects to a new node, providing me with a fresh IP Address.

It’s very easy to install NordVPN on Debian-based Distributions.


After signing up with them, you have to download the NordVPN-Repository package.

Once this is done we need to install it via Terminal:

in terminal  sudo apt-get install /home/YourUsername/Downloads/nordvpn-release_1.0.0_all.deb
in terminal  sudo apt-get update

Code language: JavaScript (javascript)
Top Things to do after installing Kali Linux

in terminal  sudo apt-get install nordvpn -Y

Code language: JavaScript (javascript)
To login you type:

nordvpn login

To connect you type:

nordvpn connect

This connects you to NordVPN. To show settings and modify them type:

nordvpn settings

_____________________________________________________________________________________________________________________________________________________________________


 Wine
------

Wine (originally an acronym for "Wine Is Not an Emulator") is a compatibility layer capable of running Windows applications on several POSIX-compliant operating
systems, such as Linux, macOS, & BSD. Instead of simulating internal Windows logic like a virtual machine or emulator, Wine translates Windows API calls into POSIX
calls on-the-fly, eliminating the performance and memory penalties of other methods and allowing you to cleanly integrate Windows applications into your desktop.

To install wine type the following command in the Terminal.

in terminal sudo apt-get install wine

_____________________________________________________________________________________________________________________________________________________________________


Terminator
-----------

Terminator is the GNU terminal emulator, which provides several features that your default terminal app does not support. It provides the ability to create
multiple terminal windows in one window and faster your work flow.
Other than that, it allows you to change other properties such as fonts, fonts color and many more. It will be useful for any Hacker or prospective PenTester.

in terminal sudo apt-get install terminator
_____________________________________________________________________________________________________________________________________________________________________

Katoolin
---------

Katoolin is a tool with which you can add and remove all the necessary Kali Linux repositories and as well as install Kali Linux tools.

in terminal sudo apt install git
in terminal sudo git clone https://github.com/LionSec/katoolin.git 
in terminal sudo cp katoolin/katoolin.py /usr/bin/katoolin
in terminal sudo chmod +x /usr/bin/katoolin
in terminal sudo katoolin

_____________________________________________________________________________________________________________________________________________________________________

GDebi Package Manager
---------------------
Kali comes with dpkg for package management but you could run into issues after installing apps because it doesn’t automatically install apps’ dependencies.

Although such issues are becoming less of a problem with workarounds like Snaps and Flatpak, most of the apps in the market are not available as sandboxed 
packages and not all apps can be installed from the software center. It is therefore important to install GDebi.

in terminal sudo apt install gdebi
_____________________________________________________________________________________________________________________________________________________________________

Software Center
---------------
The software center is a GUI app from which you can download apps online directly to your desktop. If you already have a one installed in your Kali Distro 
then you can skip this number but chances are you wouldn’t.


freestar
The good news is that you can install it using this simple command:

in terminal sudo apt install software-center

_____________________________________________________________________________________________________________________________________________________________________

Filezilla FTP Client
--------------------
If you have decided to run Kali Linux then you are likely to run some FTP-related tasks down the line and your workstation will not be complete without an 
FTP client. My pick is Filezilla and you can install it with this simple command.

in terminal sudo apt install filezilla filezilla-common -y

_____________________________________________________________________________________________________________________________________________________________________

Customization: Improve Kali Linux’s Look & Feel
------------------------------------------------

This one is a no-brainer. You need to be able to make your workstation look the way you want it to and for that, you need to install the gnome-tweaks tool, 
which is a free desktop customization and settings manager for Gnome desktops.

in terminal sudo apt install gnome-tweaks
in terminal gnome-tweaks

_____________________________________________________________________________________________________________________________________________________________________

htop 
----
This is an interactive process viewer and process manager tool, which will help you track all running background jobs and check the status of your CPU and GPU.
 
in terminal sudo apt install -y htop

_____________________________________________________________________________________________________________________________________________________________________

gotop
-----
gotop is the terminal-based graphical activity monitor. To install it we will need to use third party repository,

in terminal sudo apt install -y golang
in terminal go get github.com/cjbassi/gotop
in terminal go run github.com/cjbassi/gotop

_____________________________________________________________________________________________________________________________________________________________________

neofetch
---------
neofetch is the command line system informational tool.

in terminal sudo apt install -y neofetch

_____________________________________________________________________________________________________________________________________________________________________

lolcat
------
lolcat is the tool to give unique look to your terminal. Adds a stunning rainbow effect to its output.

in terminal sudo apt install -y lolcat
_____________________________________________________________________________________________________________________________________________________________________
