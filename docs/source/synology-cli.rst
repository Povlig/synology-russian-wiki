================================
Интерфейс командной строки (CLI)
================================


Overview: What is CLI, how do I access it, SSH or Telnet?
---------------------------------------------------------

What is the Command Line Interface (CLI)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The CLI is a Linux "shell" (a prompt based environment) provided by the Linux operating system running on the Synology Server to enable you to manage it at the Linux environment level. It is very similar to (but more powerful than) the old "DOS" environment for PC's

How do I access it
~~~~~~~~~~~~~~~~~~
To access the CLI you need to connect to the Synology Server using shell client software on your PC. Synology supports two methods (protocols) for the shell client to connect to the Synology Server, they are SSH and Telnet. The Synology Servers as supplied by Synology disable both SSH and Telnet. On firmware version 637 upwards you can enable the CLI using the Synology Servers own Web page based management GUI. For older versions of firmware (those prior to 637) Synology supply software patches for you to enable SSH and/or Telnet if you want to. Before you enable the CLI you should be aware this is defined by Synology as "Modifying" your product in software terms and therefore you may forfeit your right to software support as detailed in General Disclaimer on Modifying the Synology Server.
For instructions on how to enable CLI see Enabling the Command Line Interface

Which should I use, SSH or Telnet
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
SSH is generally a better option as it encrypts communication between your PC and the Synology Server making it very difficult for others to gain access to your passwords and see what you are doing. However windows PC's do not come with a SSH compatible shell application, so you would need to install one, a popular free SSH shell client is Putty as detailed on the Enabling the Command Line Interface page.
Telnet does not encrypt the data between your PC and the Synology Server, consequently your login password for the server is passed as "free text" and hence is visible to anyone "sniffing" the communication packets. However, if you only ever use it in a closed network you consider safe then this may not be an issue for you. Most PC's including Windows come with Telnet client software.
It is the Authors recommendation that you always use data encryption for passwords, consequently the author recommends you use SSH and install an SSH client like Putty if needed.