Technical Trends in Phishing Attacks
=========

Jason Milletary, CERT Coordination Center

##Goals and Contribution
- Identify several of the technical capabilities that are used to conduct phishing scams
- Review the trends in these capabilities over the past two years
- Discuss currently deployed countermeasures.

##Background
- focus on crimes targeting personal information used for financial fraud and identity theft
- Criminals are able to profit from the increased adoption of online services for many day-to-day activities (unawareness of threat and policy, criminals’ technical sophistication)

##Physhing Today
- Originally
 - use of electronic mail messages, designed to look like messages from a trusted agent
- Recently
 - encompass a wider variety of electronic financial crimes (+spyware)


##Tackle Box
###1. Bots/Botnets

- Bots : programs that reside on a computer and provide remote command and control access via a variety of protocols  
- Botnet : Several of these bots are under common control

 Bots provide the controller with features that can be used to support illicit activity


###2. Phishing Kits

 ready-to-use phishing kits containing items such as pre-generated HTML pages and emails

###3. Technical Deceit
- Basic URL Obfuscation
 - simple HTML redirection  
 - Use of JPEG images  
 - Use of alternate encoding schemes  
 - Registration of similar domain names  
- Web Browser Spoofing Vulnerabilities
- International Domain Names (IDN) Abuse
- Web Browser Cross-Zone Vulnerabilities

###4. Session Hijacking
- Domain Name Resolving Attacks  
 : add bogus entries to a computer's hosts file, subvert process of mapping domain names to IP addresses to forcefully redirect users to a malicious site
- Cross-Site Scripting Attacks  
 : construct a URL that contain code, such as JavaScript, that could target account credentials or involve the exploitation of vulnerable URL redirector programs
- Domain Name Typos  
 : registration of domain names that closely resemble the domain name of a legitimate high-traffic site
- Man-in-the-Middle Attacks  
 : a broad class of potential attacks in which an attacker is able to intercept, read, and modify communications between two other parties without their knowledge

###5. Abuse of Domain Name Service (DNS)
- providing phishers with the ability to easily redirect traffic from one phishing site to another if the initial site is shut down

###6. Specialized Malware
- Electronic Surveillance  
 : capture and record a user's keystrokes and mouse clicks, and also capture network packets or protocol information before it is encrypted for transit over the network
- Password Harvesters  
 : be able to search a computer for account and password
- Self-Contained Scam Pages and Dialog Boxes  
 : monitor for connections to specific banking URLs and either display a pop-up window or dialog box, or attempt to overlay the existing web page with a fake one.
- Account Siphoners  
 : actively steal money from a financial services site by automating a monetary transfer from the victim's account
- Phishing-Related Malware Examples
 - Bancos  
 : one of the oldest and largest categories of phishing malware. Bancos monitors IE for specific bank URLs and attempts to capture account information.
 - Bankash  
 : implemented as an Internet Explorer Browser Helper Object and targets online banking information.
 - W32/Grams  
 : an account siphoner that uses COM automation to directly steal money from a victim's account on an online financial site.
 - CoreFloo(AFCore)  
 : a bot that gains remote command and control of an infected computer, the ability to monitor for HTTP traffic to specified URLs.


##Phishing Countermeasures
* Widely Implemented Countermeasures
 - Awareness and Education
 - Targeting Hosting Sites
 - Web Browser Toolbars
 - Strong Authentication and Authorization
 - Virus, Spyware, and Spam Prevention
* Recommendations
 - Awareness
 - Vigilance
 - Foresight


