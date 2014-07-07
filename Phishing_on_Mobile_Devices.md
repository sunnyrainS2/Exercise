Phishing on Mobile Devices
====
Adrienne Porter Felt, David Wagner

## The contributions of this paper are:
> 1. Discuss phishing attacks between mobile applications and web sites for the first time.
> 2. Present data on how mobile applications and web sites interact.
> 3. Present and evaluate 15 types of phishing attacks.(including novel and known attacks).

## Background
  In this paper, authors focus on the two most popular modern smartphone operationg systems, Android and iOS.
  Here is the need-to-know information for this paper.

#### 1. User Interfaces on Mobile Devices
  Smartphone operating systems and browsers have minimalist user interfaces to make the size of mobile devices small.
  This leads to lack of application identity indicators in their UI.
  So a user cannot reliably tell what application is currently running or what web site is currently loaded in the browser.
  Actually, only one mobile application can control the screen at a time,
  and mobile browsers display only one browser window at a time.
  
#### 2. Platform Security
  Mobile applications are less trusted than their desktop cuonterparts.
  Applications are isolated from each other by default.
  Google and Apple prevent users from installing malware by controlling how users install applications.
  
#### 3. Control Transfers
  A control transfer occurs when the foreground application or web site changes.
  This can happen in four ways, classified according to whether the sender and target are mobile applications or web sites:
  - Mobile Sender ⇒ Mobile Target
  - Mobile Sender ⇒ Web Target
  - Web Sender ⇒ Mobile Target
  - Web Sender ⇒ Web Target

## Common Control Transfers
### Mobile Sender
  This paper studied the control transfer pattenrs of 50 most popular free Android and iOS applications and also observed whether each control transfer involves the entry of information pertaining to passwords and payment.
#### Mobile Sender ⇒ Mobile Target
  Users of mobile applications are accustomed to seeing links to other mobile applications for social sharing, upgrades, music, and credits. Links to e-mail, Facebook, Twitter, and the platform stores are particularly prevalent.

#### Mobile Sender ⇒ Web Target
  Users who participate in social sharing are at a high risk for falling for a phishing attack. Also, popular mobile applications do not commonly link users to web sites for payment.

### Web Sender
  For each domain, they collected the links on the home page and one representative page of content, as linked off the home page. In order to collect the links, we built a Firefox extension to crawl each loaded page and find link target values. 

#### Web Sender ⇒ Mobile Target
  If the application is not installed, a link to a mobile application could fail. Sometimes, web sites often link users to the Apple App Store or Android Market to install the company’s mobile application. Web sites commonly link to mobile e-mail and Twitter.  applications. Twitter, in particular, is an attractive phishing target.

#### Web Sender ⇒ Web Target
  Web-to-web links are a standard part of the Internet. So this paper did not measure their use in data set.


## Phishing Attacks
  For each scenario, we present two types of attacks: *direct attacks* and *man-in-the-middle attacks*. In a direct attack, the sender application is malicious and loads a fraudulent target application. In a man-in-the-middle attack, the sender and target applications are both benign, but a malicious party intercepts the control transfer and responds in place of the legitimate target.  
  The goal of our attacker is to mimic the legitimate application behavior that we identified in the application survey. This paper evaluate how well each attack meets these accuracy goals.

### Mobile Sender ⇒ Mobile Target
##### 1) Direct Attack
  Mobile login screens are often very simple, which makes them easy to copy. Android’s permission system would do little to warn users of this attack. The Apple application review process might prevent this attack from appearing in the App Store if reviewers detect the fraudulent screen.

##### 2) Man in the Middle
  Man-in-the-middle attacks can be launched on mobile applications in two ways: scheme squatting, 


### Mobile Sender ⇒ Web Target
##### 1) Direct Attack
##### 2) Man in the Middle
### Web Sender ⇒ Mobile Target
##### 1) Direct Attack
##### 2) Man in the Middle
### Web Sender ⇒ Web Target
##### 1) Direct Attack
##### 2) Man in the Middle


## Risk Evaluation
  An attack's plausibility is a combination of how prevalent the legitimate behavior is in real applications, and how accurately the attacker can copy the legitimate behavior. As the result of matching and evaluating each attack technique, of the 15 attacks, 8 mimic common legitimate behaviors and use highly accurate techniques.  
  In this section, identify the password-protected applications that are linked to the most often by the applications in our data set. These target applications are at the highest risk of phishing attacks because legitimate links to them are so common. Facebook and Twitter are the most common legitimate link targets.
 
## Attack Prevention
  Here are some two solutions for the problems due to the absence of identity indicators.
  > 1. permanently dedicate some small portion of the screen to application identity.  
  > 2. support a trusted password entry mechanism.  
  > 3. stop using embedded login forms which exacerbate the problem of training users to ignore security indicators.  
