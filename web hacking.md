## How do websites work?

- **When you access a website or click a link, it will send a HTTP request to the server and get the copy of the website files to the client this is called HTTP Response.**
## URL and URI
- URI identifies: a resource and differentiates it from others by using a name, location, or both.
- URL identifies: (universal resouce locater) the web address or location of a unique resource.
- URI contains components like a scheme, authority, path, and query.
- URL has similar components to a URI, but its authority consists of a domain name and port.
- A URI aims to identify a resource and differentiate it from other resources by using the name of the resource or location of the resource.
- A URL aims to find the location or address of a resource on the web.
- An Example: of a URI can be ``ISBN 0-486-35557-4.``
- An Example: of an URL is ``https://www.javatpoint.com.`` Parts of URL
A URL consists of five parts:   Example we use : ``https://blog.hubspot.com/marketing``
1.  Scheme: tells web servers which protocol to use when it accesses a page on your website example according to give ``https://`` is scheme
2.  Subdomain: is acording to example ``blog`` is subdomain
- a) If your website is like a house, your subdomains are like specific rooms in that house.
- b) A subdomain in a URL indicates which particular page of your website the web browser should serve up.
- c) For instance, subdomains like “blog” or “offers” will provide your website’s blog page or offers page.
- d) Subdomains also bucket your website into its main content categories and shows Google and your visitors that there's more information on your site than just a homepage. ( meet, docs, google.com ).
3. Top-level domain: specifies what type of entity your organization registers as on the internet.
- a) Generic Top level domain(gTLD): .gov .org .net
- b) Country code Top-level domain(ccTLD): .et .ru
4. Second-level domain: is the name of your website according to the given exaple ``hubsport`` is second-level domain
5. Subdirectory: also known as a subfolder,helps people understand which particular section of a webpage they’re on  according to the given example ``/marketing`` is subdirectory.

  ## DNS
- The Domain Name System (DNS) is the phonebook of the Internet.
- When users type domain names such as ‘google.com’ or ‘nytimes.com’ into web browsers, DNS is responsible for finding the correct IP address for those sites.
- Browsers then use those addresses to communicate with origin servers or CDN edge servers to access website information.
- This all happens thanks to DNS servers: machines dedicated to answering DNS queries.


- The DNS request the goes out from our computer is called **“DNS query”**.
- there are four servers that work together to deliver an IP address to the client: recursive resolvers, root nameservers, TLD nameservers, and authoritative nameservers.

## DNS Records
- DNS records (aka zone files) are instructions that live in authoritative DNS servers and provide information about a domain including what IP address is associated with that domain
and how to handle requests for that domain.
- These records consist of a series of text files written in what is known as DNS syntax.
- To Access DNS Record on linux we can use tools like
-           Nslookup example.com
-           Dig example.com
-           Host example.com
-           Dig example.com
-           Nslookup example.com
-           host example.com
## Types of DNS records
- **There are Many DNS record Types but lets see some**
## A Record ( Address )
- This is a Record on the server that holds IPv4 Address. 
- AAAA Record (Quad Address)
- This holds the IPv6 Of the Domain MX Record ( Mail Exchange )
- Directs mail to an email server.
- NS Record ( Name Server )
- Returns the DNS servers (nameservers) of the domain. Server Where all the DNS records are stored!



- As the name suggests HTTP requests are a request which the browser sends to the server
- HTTP responses are a response from the server to the browser.
- The requests and Response are sent and received with a Header.
## HTTP Headers
- The HTTP headers are used to pass information between the clients and the server through the request and response header.
- All the headers are case-insensitive, headers fields are separated by colon, key-value pairs in clear-text string format.
- The end of the header section denoted by an empty field header(New line).


## Types of Headers
- **General Header:** This type of headers applied on Request and Response headers both but without affecting the database body.
- **Request Header:** This type of headers contains information about the fetched request by the client.
- **Response Header:** This type of headers contains the location of the source that has been requested by the client.
- **Entity Header:** This type of headers contains the information about the body of the resources like Content-length.
## Request Headers
- This is A header sent to the server.
- In Request Header There are different kind of headers
- Example: GET, Host, Cookie,...

#### The 1st line Contains
- Request Method
- **Path:** *The path where the file/folder is located*
- **Protocol Type:** *which HTTP protocol ( HTTP 1 , HTTP/1.1 , HTTP/2)*
#### The 2nd line
- **Host:** *the website link*
#### The 3rd line
- **Cookie:** *used to check a user*
#### The 4th line
- **User-Agent:** *used to place the browser information*

## Response Header
- This is response from The server to the browser
#### 1st line
- **HTTP:** *Tells the server Protocol*
- **Status Code**
#### 2nd line
- **Date:**  *Date of the response sent*
#### 3rd line
- **Content-Type:** *What type of content the server sent*
- **Encode type:**  *used for encode responses*
#### 4th line
- **Content-length:** *The number of the alphanumeric and spaces*
####  5th line
- **Server:** *type of the webserver*
#### 6th line
- **This line is empty used to show that the headersending.** 
- And begining of the body
## 7th…. Line
- The html content


## HTTP request methods
- The method designates the type of request being made to the web server.
- The most common types of request methods are GET and POST but there are many others,
- It including HEAD, PUT, DELETE, CONNECT, and OPTIONS.
- GET and POST are widely supported while support for other methods is sometimes limited but expanding.
## Methods and their defnetioon
- **GET :** *Request for resource from server*
- **POST :** *submit data to server*
- **HEAD :** *same as GET but does not return the body*
- **PUT :** *The data witin requset must be stored at the URL supplied, replace any exist data*
- **DELETE :** *Delete resource*
- **OPTIONS :** *Return the HTTP methods supported by the server*
- **CONECT:** *client requests the HTTP proxy to forward a TCP connection o some distination.  and usedd to creat a Tcp/Ip tunnel connecion using HTTP proxies*
## GET vs POST on URL
1. **GET Requests -**      Example:
-      htttps://example.come/login?username=yared&passwodr=yared123
- In this cause Username and Password are  called **Parameters.**

2. **POST Request -**  Example: https://example.com 
```
       POST /login HTTP/1.1
       HOST: example.com
       ..
       ..
       ..
      Usename=yared&password=yared123

```


## HTTP Status Code
- The Status-Code element in a server response
- is a 3-digit integer where the first digit of the Status-Code defines the class of response and the last two digits do not have any categorization role.
- There are 5 values for the first digit:
- **1xx:** **Informational**
■ It means the request has been received and the process is continuing.
- **2xx: Success**
- **It means the action was successfully received, understood, and accepted.**
**-** **3xx: Redirection**
- **It means further action must be taken in order to complete the request.**
**-* **4xx: Client Error**
- **It means the request contains incorrect syntax or cannot be fulfilled.**
**-** **5xx: Server Error**
- **It means the server failed to fulfill an apparently valid request.**
#### Some common codes
- **200** = *request is Successful( OK )*
- **301** = The requested page has moved to a new url . ( Moved Permanently )
- **302** = *The requested page has moved temporarily to a new url .( Found ) => when there is redirection*
- **400** = *The server did not understand the request. (Bad Request)*
- **401** = *The requested page needs a username and a password. (Unauthorized).*
- **403** = *Access is forbidden to the requested page.(Forbidden).*
- **404* = *The server can not find the requested page.(Not Found)*
- **405** = *The method specified in the request is not allowed.(Method Not Allowed)*
- **500**= *The request was not completed. The server met an unexpected condition.(Internal Server Error)*



- The headers are shown on some methods.
1. Developers tool(on browser)
2. Curl
3. Burp suite
## Developers tool
- To open it on browser
- Press ``Ctrl+shift+C`` or > right click on the page  > select inspect >click inspect and you see developer tools
- **This tools contains lot of things**
1. **Inspector:** *to see and edit the HTML and CSS temporarly*
2. **Console:** *to run some Javascript codes*
3. **Debugger:** *used to do debug in runtime*
4. **Network:** *to see the requests and responses*
5. **Storage:** *to store catch and cookies*
6. **Network:** *to network concted service*

 ## Curl on linux
- **CURL, which stands for client URL, is a command line tool that developers use to transfer data to and from a server.**
- At the most fundamental, cURL lets you talk to a server by specifying the location (in the form of a URL) and the data you
want to send.
- cURL supports several different protocols, including HTTP and HTTPS, and runs on almost every platform.
- This makes cURL ideal for testing communication from almost any device (as long as it has a command line and network
connectivity) from a local server to most edge devices.
- ``Syntax: curl [options] [URL]``
#### Options
- **To get we content of site** 
-       curl https://example.com
- **To change request method**
-        curl -x GET https://example.com
- **To see the response headers**
-         curl -I https://example.com


## Burp suite
- Burp or Burp Suite is a set of tools used for penetration testing of web applications.
- It is developed by the company named Portswigger, which is also the alias of its founder Dafydd Stuttard.
- BurpSuite aims to be an all in one set of tools and its capabilities can be enhanced by installing add-ons that are called BApps.
- Burp Suite is an integrated platform and graphical tool for performing security testing of web applications
- it supports the entire testing process, from initial mapping and analysis of an application's attack surface, through to finding and exploiting security vulnerabilities.
- It have a lot of tools all together.
- Simply Help Hackers To Act like A Proxy, it will intercept A request,


## OWASP Top 10
- OWASP Stands for **Open Web Application Security Project.**
- The OWASP Top 10 is a standard awareness document for developers and web application security.
- It represents about the most critical security risks to web applications.
- Globally recognized by developers as the first step towards more secure coding.
- This Project Releases Top 10 risky vulns every 4 years.
- Detail:(!checkthis[https://owasp.org/Top10/])
- OWASP also releases API vulnerabilities
- This is the OWASP’s Top 10 Vulns reported in 2021
- Each Vulnerabilities are Detailed.

 #### Let us see some Common web Vulnerabilities

## Brute force attack
- **Brute-Force Attack:** *In a brute-force attack, an attacker systematically tries all possible combinations of characters until the correct password is found.*
-  It starts with the simplest and shortest passwords and incrementally tries longer and more complex combinations.
-  Brute-force attacks are exhaustive in nature and do not rely on any specific information about the target or common password patterns.
-  This method can be time-consuming and computationally intensive, especially for longer passwords or strong encryption algorithms.

## Dictionary Attack:
- **A dictionary attack:** *on the other hand, relies on a predefined list of words, phrases, or commonly used passwords called a "dictionary" or "word list".*
- The attacker systematically tries each word in the list as a potential password. 
- This approach is effective when the targeted password is a common word, a name, a simple combination of words, or a commonly used password. 
- Dictionary attacks are faster compared to brute-force attacks because they do not need to try every possible combination of characters.



## XSS
- It is included in Injection Bug
- XSS/ Cross site scripting/ is a vulnerability that leads to a lot of huge attacks.
- This Bug is exploited. As the following
- If there is a search place and the search place expects a text to search and displays below.
- But if we add some html/JS codes on that place, this means it will add the code to the innerHTML
- SO our code will be executed!
## Cross-Site Scripting
- allows attackers to inject malicious scripts into web pages viewed by other users.
S
...
- This is Simple Demo,
But Attacker can Use
this injection attack
to access your
authentication tokens,
Session IDs
- They can Use this and
Hook your browser with
tool called “BeefXSS”
REMEMBER
All the Injection Attacks are done on some Parameter.
SQL injection
● It is included in Injection Bug
● It is same with xss, but here we will add a
sql code to the search place.
● SQL is a query language used in Back end
to retrieve data from database.
● Most of the time used to bypass login
pages.
## SQL Injection
Attackers Use this Vuln to manipulate or gain unauthorized access to a database.

- This is Just Demo, But this is how the Hack happens,
➔ On the payload Attackers can
Craft a SQL query that can cause
RCE, Full Database Detail
listing and much moreeeee.
Further
Learn about Tool called SQLMap.
## Rate limit
- This is a limiting problem.
- Think like if the developers did made a limit to
- some task.
- Example:
- If there is website , that send an OTP/verification code
- And if it doesn't limit to some code sends only.
- I can make the site to send 100000 OTPs to ma phone this means
- We will make the site to lose a lot of money


## Foothold
There are some tools, used to Crack Passwords of Files, Hashes
- Hashcat
- John The Ripper
- More..
Try to Learn These tools for further System hacking Potential
- learn in youTube [https://www.youtube.com/watch?v=5fy6Lq1vgZk&pp=ygUHSGFzaGNhdA%3D%3D]
- learn on youTube [https://www.youtube.com/watch?v=XjVYl1Ts6XI&pp=ygUQam9obiB0aGUgcmlwcGVyIA%3D]
