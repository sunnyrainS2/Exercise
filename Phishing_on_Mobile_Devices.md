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

## Phishing Attacks

## Risk Evaluation

## Attack Prevention
  Here are some two solutions for the problems due to the absence of identity indicators.
  > 1. permanently dedicate some small portion of the screen to application identity.  
  > 2. support a trusted password entry mechanism.  
  > 3. stop using embedded login forms which exacerbate the problem of training users to ignore security indicators.  
