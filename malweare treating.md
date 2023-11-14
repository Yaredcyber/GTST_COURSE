
## What is Malware
- A Malware is a set of instructions(program) that run on your computer and make your system do 
something that an attacker wants it to do.
- The name Malware Come from
- Malicious => ተንኮለኛ(bad thing)
- Software => set of instruction(program)
### Mal - ware 
What malwares do?
1. Removing data/files
2. Encrypting data/files
3. Corrupting data/files
4. Stealing Data/files
5. Spying on user
6. …
- Kinds of Malwares
- Based on their propagation/infection and attack, there are many kinds of malwares.
1. Trojan
2. Worm
3. Virus
4. Ransomware
5. Rootkit
6. Adware
7. ...
## TROJAN!
- Trojan, is a type of malicious code or software that looks legitimate but can take control of your computer. 
- A Trojan is designed to damage, disrupt, steal, or in general inflict some other harmful action on your data or network.
- They don’t replicate.
- The name Trojan came from the Greek mythology Trojan Horse.
- Trojans will looks normal or legit software and then BOOM!
### Greek Mythology 
- There was war between 2 countries and the winning country, send gift to the losing country the gift was huge wood house. 
- But inside it there were soldiers and the soldiers came out at night and evade the city. 
### Common types of trojan
1. Backdoor Trojan
- a. This Trojan can create a “የጀርባ በር” on your computer. 
- It lets an attacker access your computer and control it. Your data can be downloaded by a third party and stolen. 
- Or more malware can be uploaded to your device.
2. Mailfinder Trojan
- a. This Trojan seeks to steal the email addresses you’ve accumulated on your device.
3. Remote Access Trojan
- a. This Trojan can give an attacker full control over your computer via a remote network connection. 
- Its uses include stealing your information or spying on you.
4. Trojan banker
- a. This Trojan takes aim at your financial accounts. It’s designed to steal your account information for all the things you do online
- That includes banking, credit card, and bill pay data.
## Worm
- A computer worm can propagate or self-replicate from one computer to another without human interaction after breaching a system. 
- Typically, a worm spreads across a network through your Internet or LAN (Local Area Network) connection.
- Damages files on the system and the systemVirus
- They are the older and famous ones
- Virus is a program written to enter to your computer and damage/alter 
### your files/data. 
- A virus might corrupt or delete data on your computer. 
- Viruses can also replicate themselves. 
- A computer Virus is more dangerous makes changes or deletes your files Common signs of virus infection
- Speed of System
- Pop-up windows
- Self-executing
- Account being log out
- Crashing of device
- Mass emails being sent from you
- Files and system settings are altered.
- Common types of virus
- There are several types of computer viruses that can infect devices.
1. Resident Virus
- a. Viruses propagate themselves by infecting applications on a host computer. 
- A resident virus achieves this by infecting applications as they are opened by a user.
- A non-resident virus is capable of infecting executable files when programs are not running.
2. Multipartite Virus
- A multipartite virus uses multiple methods to infect and spread across computers.
- It will typically remain in the computer’s memory to infect the hard disk,
- Then spread through and infect more drives by altering the content of applications. 
This results in performance lag and application memory running low. 
3. Browser Hijacker
- a. A browser hijacker manually changes the settings of web browsers, such as replacing the homepage, editing the new tab 
page, and changing the default search engine. Technically, it is not a virus because it cannot infect files
## Ransomware
- Ransomware is malware that employs encryption to hold a victim’s information at ransom. 
- A user or organization’s critical data is encrypted so that they cannot access files, databases, or applications
- A ransom is then demanded to provide access.
- Ransomware is often designed to spread across a network and target database 
and file servers, and can thus quickly paralyze an entire organization.
- Ransomware => RANSOM + SOFTWARE
## Rootkit
- A rootkit is a malicious software bundle designed to give 
unauthorized access to a computer or other software. 
- Rootkits are hard to detect and can conceal their presence within an infected system. 
- Hackers use rootkit malware to remotely access your computer, manipulate it, and steal data.
## Adware
- Adware, or advertising supported software, 
- is software that displays unwanted advertisements on your computer.
- Adware programs will tend to serve you pop-up ads, can change your browser's homepage,
-  add spyware and just bombard your device with advertisements.
### How do they infect?
- USB drop attack ( infected removable drives )
- Hackers drop them around your company and 
- Spam emails
- Malicious Office macros
- Softwares/Applications from unsafe websites.
- Torrent sites
- Using Cracked Softwares
- Malicious Browser extension
- How they are hidden/undetected
####  Hackers use different methods to pass some protections and infect that system.
### 1. Packers
- a. A packer is a program that compresses an executable to make it smaller. 
- It wraps the compressed executable in the code necessary to decompress itself at runtime.
-  Packing changes this the binary patterns and some  hashes(day5) , so the AV may not detect the packed file.
### 2. Crypters/encoders
a. A crypter is similar to a packer but adds additional obfuscation or encryption to the mix.
- Like a packer, its goal is to change the binary fingerprint of a file to avoid detection.
- In a nutshell, the crypter encrypts the original executable using an encryption algorithm — often something as simple as a XOR cipher with a unique key.
### 3. Polymorphic Malware
- a. At the highest level, polymorphic malware is malware that repeatedly uses packing and crypting methods to 
change the way it looks.
 4. Downloaders, Droppers, and Staged Loading
- a. Many kinds of malware use staging programs called droppers or downloaders to learn about a system before installing the real malware.
- Some of these droppers scope out a system first to avoid triggering security alerts 
- when they download and install the real payload.
# Malware Prevention
1. Install anti-virus and anti-spyware software.
a. Example: kaspersky,avg,smadav
2. Use secure authentication methods.
a. 2-factor authentication
b. Implement email security and spam protection
3. Keep software updated
4. Use the least-privilege model.
5. Monitor for suspicious activity
6. Educate your users
## Malware in history
1. Morris Worm: Also known as the Internet worm, this was one of the 
first computer worms to spread via the Internet and earn notoriety in 
the media.
2. ILOVEYOU: The ILOVEYOU virus infected tens of millions of computers globally, resulting in billions of dollars in damage.
3. Stuxnet: Some experts believe this sophisticated worm was developed for years to launch a cyberattack.
4. WannaCry: is a ransomware which targeted computers running.
-The Microsoft Windows operating system by encrypting (locking) data and demanding ransom payments in the Bitcoin cryptocurrency.
## Python for Malware development
- As we saw malwares do so many things and we can develop that 
malware based on the algorithm, We need. 
- First we have to understand what our malware have to do.
- There are so many kinds of malware purpose
- Delete files
-  Encrypt files
-  Corrupt files

## File Handling in python
- Files are names locations on disk to store related information.
- Files Used to Store Data in Storage Devices.
- When we want to read from or write to a file, 
- we need to open it.
- And also when we are done we will close it.
- In Python ,a File Operation takes place in the following order:
- Open a File
- Read or Write(perform operation)
- Close the file
cont…
- Python has a built-in function called open().
- Syntax:
- with open(“fileName or filePath”,’x’) as var
- Modes:
- write---------------------------------w
- read---------------------------------r 
- append---------------------------a 
- Create----------------------------- x
- text mode-------------------------t 
- binary mode---------------------b
## Reading files
- To read files on python we have to open it by reading mode ’r’
- There are many methods for this. But, we can use the read 
- read() - >This read file up to the inputted size number.
- BUT if you don’t add the size it will read it until the end.
- readline() -> To read files only one line
- readlines() -> reads all file in 1 line
- Syntax:
- var.read(5)
- var.readline()
- var.readlines()
