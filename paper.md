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
- Cross-Site Scripting Attacks
- Domain Name Typos
- Man-in-the-Middle Attacks

###5. Abuse of Domain Name Service (DNS)
###6. Specialized Malware
- Electronic Surveillance
- Password Harvesters
- Self-Contained Scam Pages and Dialog Boxes
- Account Siphoners
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


