
## Anonymity
- Anony/unknown in amharic is *የማይታወቅ*
- **When Black Hat Hackers do Security tests on some target, They willbe unknown**
- This is because they are doing illegal things so they try to beanonymous/የማይታወቅ ሰው
- Keeping your identity private, but not your actions.
- For example, using a fake name to post messages to a social mediaplatform.
- Anonymity is Simply using a fake *Profile/Location/Identity/personality
Online Privacy*
- **black hat hackers use many tools and apps use for anonymity this are :-**

## Methods of Anonymity
- There are several ways to be protected or to be Anonymous on the internet.
- These methods can change our identity,location or personality.
1. Proxychains
2. Tor Network
3. VPN
4. Mac change
5. Incognito
6. Secured OS
7. Temp mail
8. Temp number
## 1. proxy server
- A proxy server is a system or router that provides a gateway between users and the internet.
- Therefore, it helps prevent cyber attackers from entering a private network.
- Proxy means intermediary/*መካከለኛ* middle 
### ProxyChains
- We have seen what proxy is so lets see what Proxy chains are.
- Proxy chain is simply a chain of proxys.
- We have a lot of proxy lists so our request will pass through lot of proxys .This will hide our IP.
- Here our 1st IP was ``70.248.28.23`` but the Internet(webserver,...) know as ``154.16.127.161``
## Types of ProxyChains
- Based on the path we follow There are 4 Types of proxychains.
1. Dynamic chain
2. Strict Chain
3. Round Robin Chain
4. Random Chain
## Dynamic Chain
- Dynamic Chaining is That way the proxy Servers are chained is as the proxy list given.
- If there is any server that is not working it will be skipped.
- If any of them doesnt work it will be broken and display errors.
## Strict Chain
- All Proxies chained in the order as the are listed.
- All proxies Have to be up and working, if 1 is not working it will display error
## Round Robin chain
- It follows the order of the proxy list
- It will skip if 1 proxy is not working
- If all the proxies not working it will start again and check them.
- This makes it different from Dynamic chain Random Chain
- It will choose some Proxy server Randomly and creates chain in random order.
- Not working will be Skipped!
- Each Request will be in random sequence of servers demo
1. Find some Proxy servers use google search (proxy)[https://geonode.com/]
2. Open ``/etc/proxychains4.conf``
3 Turn on any kind proxychain you need
4. Add “proxychains4” in front of
5. Put your proxy servers
6. Accessing with proxychains


## T.O.R/The Onion Routing/ Network
- Tor is an open-source privacy network that enables anonymous web browsing.
- The worldwide Tor computer network uses secure, encrypted protocols to ensure that users' online privacy is protected.
- Tor users' digital data and communications are shielded using a layered approach that resembles the nested layers of an onion.
- Tor uses an onion-style routing technique for transmitting data.
- When you use the Tor browser to digitally communicate or access a website, the Tor network does not directly connect your computer to that website.
- Instead, the traffic from your browser is intercepted by Tor and bounced to a random number of other Tor users’ computers before passing the request to its final website destination.


## torghost
1. Clone it from github (torghost)[ https://github.com/SusmithKrishnan/torghost]
2. Install tor
3. Open it!
- Your last Proxy IP will be shown(Public IP) VPNs
- VPN means Virtual Private Network.
- a service that helps you stay private online.
- A VPN establishes a secure, encrypted connection between your computer and the internet, providing a private tunnel for your data and communications while you use public networks
## VPN…
- There are a lot of VPNS, those are paid and free
- The paid are more secured and private, still the free are Good
- Example: Nord VPN, Proton VPN, windscribe VPN,...

…
Buying premium VPNS are good.
- Mac Changer
- As We saw MAC address can tell about our Device.
- SO , if we changed that we can change our device id.
- We can use tool called “macchanger” on kali
- 1st turn off the interface you want to change.
- Turn it on now!
- You can add your specific MAC with -m option Incognito mode
- This is a mode that browsers have.
- This will help you to have a browser with out logging your history,cookies,cache,..
- This will help you when you are try to surf some site but if you dont need the site to know your identity,
-  you can use this because it doesnt have any recording process.
-  ### let try this
  1. opean your terminal write ``sudo macchanger r wlam0/eth0`` it can generate random unknown mac adress
  2.  a) ``sudo ifconfig eth0/wlan0 down`` used for down your network
      b) ``sudo macchanger -m < your  wented mac adress> eth0/wlan0`` = used for give your interested MAC  adress.
      c) ``sudo ifconfig eth0/wlan0 up`` = used for sart your mac adresss
## Secure OS
- This are Operating systems, that have a security and privacy feature.
- *Windows and Mac OS will record some of your activity also they are not good on privacy and security.*
● There for the always Best OS Linux is always recommended when you think about privacy and Security.
## Temporary mail
- While You do some pentest you dont have to expose your email and profile for this purpose u need fake emails,
- but if you dont have to time create one you can use fake email providers.
- (tempmail)[ https://temp-mail.org/]
- It have a browser extention too

- Every server you connect to on the internet — be it a web server, a mail server, or a VPN server — can see your IP address.
- This is a number that uniquely identifies your internet connection and can be easily traced back to you.
- Achieving true anonymity on the internet therefore requires good operational security (OPSEC) on your part to ensure your real IP address is not revealed.
- Tools that can hide your IP address and protect anonymity include VPNs and the Toranonymity network, but there’s no solution that can guarantee 100% anonymity.
- Tor is sometimes considered to be more anonymous than VPNs due to its decentralized nature, but it comes at the cost of lower performance, ease of use, and stability.
- Full anonymity is difficult because you must always use anonymity tools for all aspects of your online life, as even a temporary lack of anonymity is sufficient to expose your identity.
## Deep web
- The deep web refers to all the web pages and data that are not indexed by search engines and cannot be accessed through traditional search methods.
- It includes content that is protected by passwords, databases, and other security measures.
- Examples of deep web content include private email accounts, online banking portals, subscription-based websites, and more.
- Essentially, the deep web is the part of the internet that is not easily accessible to the general public.
  ## DARK WEB
- The dark web is a part of the internet that isn't indexed by search engines.
- You've no doubt heard talk of the “dark web” as a hotbed of criminal activity
- The dark web is a small portion of the deep web that is intentionally hidden and requires specific software or configurations to access.
- It is unique type of internet world.
- Their link ends with .onion , this is because it uses TOR networks.
- Also this kinds of links won’t be opened by normal browser.
- For this purpose we need a special .onion reading browser,
 Example: Tor browser.

## DOS and DDOS Attacks
- DoS is short for Denial-of-Service attacks.
- DDoS stands for Distributed Denial-of-Service attack.
- It's used to crash a website by overwhelming the network with access requests from a computer.
- This method also crashes a targeted website and makes it unavailable to legitimate users.
- (like Mac spoofing)
- It is purposeful attack
- On DDOS, the request will be sent from DIfferent Computers/hosts this will make the attack harder.
- IT is Highly illegal!
##  Techniques:
## SYN floods
- **Sending lots of SYN**
- **Service Request floods**
- ** Create many connections**
- **Application level DOS**
- Exploiting vulns like
- Buffer Overflow
- SQL injection
## Tools For DOS
1. SolarWinds Security Event Manager (SEM)
2. ManageEngine Log360
3. HULK
4. Tor’s Hammer
5. Slowloris
6. LOIC
7. Xoic
8. DDOSIM
9. RUDY
10. PyLoris
## Prevention ways
- Have you seen Cloudflare, These pages are One of the prevention ways.
- Limit or shut off broadcast forwarding where possible
- Set up firewalls
- Eliminate and patch known vulnerabilities
- Monitor network inbound traffic
