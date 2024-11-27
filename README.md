# SSH login brute forcing

This project illustrates the process of brute-forcing SSH login credentials using Python’s pwntools and paramiko libraries. The objective is to automate the process of attempting various passwords from a wordlist to access an SSH server. The script loads passwords from a file, tries each one for login, and identifies the correct password by handling exceptions caused by failed authentication attempts.

This project replicates a common security testing scenario, where penetration testers perform brute-force attacks to evaluate the strength of system authentication. It offers a practical learning experience in understanding how brute-force attacks are carried out and highlights how systems can be vulnerable to such attacks when robust password policies are not implemented.

To enable SSH on my Kali Linux machine, I ran sudo systemctl start ssh to start the service. I then checked its status with sudo systemctl status ssh and verified it was listening on port 22 using sudo netstat -tuln | grep :22


sudo systemctl start ssh
sudo systemctl status ssh
sudo netstat -tuln | grep 22




_______________________________________________
Project Overview

1 create a script 
to find top 10000 password you can download here https://github.com/danielmiessler/SecLists/tree/master/Passwords/Common-Credentials
2 enable ssh on a local host 
3 run script 
4 once our script identify valid password it stops and show as 
5 here is an example of using existing python modules - pwn and paramiko to perform common hacking task of brute forcing


Conclusion
