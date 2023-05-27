# How_To_Create_An_Ubuntu_Remote_Desktop_Connection
First, you need to have created an Ubuntu ec2 instance and connected to it via SSH or session manager in order to run the series of commands that follow.

### The provided lines of code are a series of commands that are commonly used in Ubuntu or Debian-based Linux systems. Let's go through each command and explain its purpose:

```sudo apt-get update```
This command updates the package lists on your system. It fetches information about the latest versions of packages available from the software repositories.

```sudo apt install xrdp```
This command installs the XRDP package, which stands for X Remote Desktop Protocol. XRDP allows you to connect to your Ubuntu system remotely using the Remote Desktop Protocol.

```sudo systemctl enable xrdp```
This command enables the XRDP service to start automatically when the system boots up. It ensures that the XRDP service remains active and available.

```sudo apt-get dist-upgrade```
This command performs a distribution upgrade of your system. It upgrades installed packages, including their dependencies, to the latest available versions. It is a more extensive upgrade than a regular package upgrade.

```sudo add-apt-repository ppa:gnome3-team/gnome3```
This command adds a Personal Package Archive (PPA) repository to your system. The specified repository in this case is the GNOME3 Team's PPA, which provides the latest GNOME desktop environment packages.

```sudo apt update```
This command updates the package lists again after adding the new repository (GNOME3 Team's PPA) in the previous step. It fetches information about the packages available from the added repository.

```sudo apt-get install gnome-shell ubuntu-gnome-desktop```
This command installs the GNOME Shell and the Ubuntu GNOME desktop packages. It sets up the GNOME desktop environment as an alternative option to the default desktop environment on your Ubuntu system.

```sudo apt-get update```
This command updates the package lists once again after installing the GNOME Shell and Ubuntu GNOME desktop packages.

```sudo passwd ubuntu```
This command sets a new password for the user account named "ubuntu." It prompts you to enter and confirm the new password.


### Logging into the machine via RDP
Once you're done configuring your resources via SSH, now it's time to try to access the server via RDP.

Just open Remote Deesktop Protocol from your start menu on your Windows machine,
![ipAddressRDP](https://github.com/evans-kithinji/How_To_Create_An_Ubuntu_Remote_Desktop_Connection/assets/105270837/85aceaf1-d7bc-4949-a84d-38f1eae722f6)

then connect using your IP address.

When prompted for a username and password, use 'ubuntu' for username and the password that you set earlier on.




### Video Tutorial on How to setup GUI Desktop with Ubuntu on AWS EC2
https://youtu.be/PBKmTRz_2R4



