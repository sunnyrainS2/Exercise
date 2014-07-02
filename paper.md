Technical Trends in Phishing Attacks
=========

Jason Milletary, CERT Coordination Center

##Goals and contributions
The goals and contributions of this paper are three-fold.
> - Identify several of the technical capabilities that are used to conduct phishing scams
> - Review the trends in these capabilities over the past two years
> - Discuss currently deployed countermeasures.

##Background
- This paper focus on crimes targeting personal information used for financial fraud and identity theft.
- Criminals are able to profit from the increased adoption of online services for many day-to-day activities. There are three major factors that criminals have been able to take advantage of : unawareness of threat, unawareness of policy, and criminals’ technical sophistication
- Originally, physhing was identified as the use of electronic mail messages, designed to look like messages from a trusted agent. Over time, these fake emails and web sites have evolved to become more technically deceiving to casual investigation. Recently the definition of phishing has grown to encompass a wider variety of electronic financial crimes including spyware.


##Tackle box: Tools for Phishing
Just as with real fisherman, phishers today have a large tackle box of tools available to them.
These tools serve a variety of functions, and in this paper, they are classified into six broad categories.

####1. Bots/Botnets
 "Bots" refer to programs that reside on a computer and provide remote command and control access via a variety of protocols. 
When Several of these bots are under common control, it is commonly referred to as a botnet. Bots provide the controller with features that can be used to support illicit activity such as DDos(Distributed denial of service).


####2. Phishing Kits
 Ready-to-use phishing kits containing items such as pre-generated HTML pages and emails provide a lower barrier to entry into the marketplace for criminals.

####3. Technical Deceit
- **Basic URL Obfuscation** : URL obfuscation misleads the victims into thinking that a web site is a trusted site. These following methods tend to be technically simple yet highly effective, and are still used to some extent in phishing emails today.
 - simple HTML redirection  
   : use a legitimate URL within an anchor element but have its href attribute point to a malicious site
 - Use of JPEG images  
   : JPEG image appears to be legitimate email, however when users click on this image, they are directed to a phishing site.
 - Use of alternate encoding schemes  
   : be observed in cross-site scripting attacks to obfuscate the malicious URL
 - Registration of similar domain names  
   : trick customers who are satisfied by just seeing a legitimate name appear in a URL
- **Web Browser Spoofing Vulnerabilities**  
 : several vulnerabilities in web browsers have provided phishers with the ability to obfuscate URLs and/or install malware on victim machines
- **International Domain Names (IDN) Abuse**  
 : mechanism by which domain names with Unicode characters can be supported in the ASCII format used by the existing DNS infrastructure
- **Web Browser Cross-Zone Vulnerabilities**  
 : attempt to lure users to a web site attempting to install spyware and/or malware onto the victim's computer, and theses web sites usually rely on vulnerabilities in web browsers even when these sites are located in a security zone

####4. Session Hijacking
- **Domain Name Resolving Attacks**  
 : add bogus entries to a computer's hosts file, subvert process of mapping domain names to IP addresses to forcefully redirect users to a malicious site
- **Cross-Site Scripting Attacks**  
 : construct a URL that contain code, such as JavaScript, that could target account credentials or involve the exploitation of vulnerable URL redirector programs
- **Domain Name Typos**  
 : registration of domain names that closely resemble the domain name of a legitimate high-traffic site
- **Man-in-the-Middle Attacks**  
 : a broad class of potential attacks in which an attacker is able to intercept, read, and modify communications between two other parties without their knowledge

####5. Abuse of Domain Name Service (DNS)

 Dynamic DNS providers providie phishers with the ability to easily redirect traffic from one phishing site to another if the initial site is shut down. Thus, The use of dynamic DNS and registration of multiple IP addresses for a single fully qualified domain name (FQDN) is becoming more prevalent to increase the resilience of phishing sites.

####6. Specialized Malware
- *Electronic Surveillance* : capture and record a user's keystrokes and mouse clicks, and also capture network packets or protocol information before it is encrypted for transit over the network
- *Password Harvesters* : be able to search a computer for account and password
- *Self-Contained Scam Pages and Dialog Boxes* : monitor for connections to specific banking URLs and either display a pop-up window or dialog box, or attempt to overlay the existing web page with a fake one.
- *Account Siphoners* : actively steal money from a financial services site by automating a monetary transfer from the victim's account
- Phishing-Related Malware Examples
 - *Bancos*  
 : one of the oldest and largest categories of phishing malware. Bancos monitors IE for specific bank URLs and attempts to capture account information.
 - *Bankash*  
 : implemented as an Internet Explorer Browser Helper Object and targets online banking information.
 - *W32/Grams*  
 : an account siphoner that uses COM automation to directly steal money from a victim's account on an online financial site.
 - *CoreFloo(AFCore)*  
 : a bot that gains remote command and control of an infected computer, the ability to monitor for HTTP traffic to specified URLs.


##Good ways to deal with phishing attacks
Various solutions have been developed in response to phishing.
The following list contains five most commonly implemented today:
 > 1. Awareness and Education
 > 2. Targeting Hosting Sites
 > 3. Web Browser Toolbars
 > 4. Strong Authentication and Authorization
 > 5. Virus, Spyware, and Spam Prevention

  And Here are some recommendations of this paper to help people deal with the increasing technical capabilities of criminals conducting phishing scams.  
  First, phishing **awareness** must continue to evolve to address the growing capabilities available to phishers. Second, decrease the return on investment of the activity to the criminal community for **vigilance**. Third, having **foresight** is important to be aware of when sensitive information is at risk.
