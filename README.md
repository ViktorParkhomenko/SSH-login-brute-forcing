# SSH login brute forcing

This project illustrates the process of brute-forcing SSH login credentials using Python’s pwntools and paramiko libraries. The objective is to automate the process of attempting various passwords from a wordlist to access an SSH server. The script loads passwords from a file, tries each one for login, and identifies the correct password by handling exceptions caused by failed authentication attempts.

This project replicates a common security testing scenario, where penetration testers perform brute-force attacks to evaluate the strength of system authentication. It offers a practical learning experience in understanding how brute-force attacks are carried out and highlights how systems can be vulnerable to such attacks when robust password policies are not implemented.

To enable SSH on a Kali Linux machine, run the following commands:

Start the SSH service with sudo systemctl start ssh.
Check the status of the service using sudo systemctl status ssh.
Verify SSH is listening on port 22 by running sudo netstat -tuln | grep :22.
These steps ensure that SSH is running and accessible on the local machine.
![Screenshot_2024-11-27_13-44-07](https://github.com/user-attachments/assets/c522aa48-f008-4882-9e29-896688024fd6)

Here is an example of using the existing Python modules pwn and paramiko to perform the common hacking task of brute forcing.
![Screenshot_2024-11-27_14-31-20](https://github.com/user-attachments/assets/d016d4f8-85f9-427a-a0f3-53fe566aa47b)

from pwn import * imports all functions and classes from the pwntools library, which is commonly used for exploit development and CTF (Capture The Flag) challenges. It provides easy access to functions for networking, binary exploitation, and interacting with remote services.

import paramiko imports the paramiko library, which is used for SSH connections in Python. It allows you to create, manage, and automate SSH sessions, making it useful for tasks like remote server administration and brute-forcing SSH login credentials.

host = "127.0.0.1": Specifies the target SSH server's IP address (localhost, in this case). This script is testing the SSH server running on the same machine.
username = "kali": Defines the username to use for the SSH login attempts. The username remains constant throughout the brute-force process.
attempts = 0: Initializes a counter to keep track of how many password attempts have been made.

The top 10,000 passwords are available for download on GitHub: https://github.com/danielmiessler/SecLists/tree/master/Passwords/Common-Credentials







_______________________________________________
Project Overview

1 create a script 
to find top 10000 password you can download here https://github.com/danielmiessler/SecLists/tree/master/Passwords/Common-Credentials
2 enable ssh on a local host 
3 run script 
4 once our script identify valid password it stops and show as 
5 here is an example of using existing python modules - pwn and paramiko to perform common hacking task of brute forcing


Conclusion
