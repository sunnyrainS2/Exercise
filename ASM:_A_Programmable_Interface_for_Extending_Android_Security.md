# ASM: A Programmable Interface for Extending Android Security.
Nadkarni, Adwait, and William Enck. 2014.

### Goal and contributions

##### Goal
to promote OS security extensibility in the Android platform

##### Contributions
1) identify the authorization hook semantics required for new operating systems such as Android.
2) design and implement the extensible Android Security Modules (ASM) framework.
3) implement two example ASM apps to demonstrate the utility of the ASM framework.


### Background
Android defines four types of components: *activity*, *service*, *broadcast receiver*, and *content provider*.


### Design Goals

1) Generic authorization expressibility
2) Ensure existing security quarantees
3) Protect kernel integrity
4) ultiple authorization modules
5) Minimize resource overhead


### Android security enhancements

System | security enhancements | Note
------ | --------------------- | ----
Kirin | place constraints on permissions of applications being installed | 
Saint | mediate communication between components in different applications | 
XManDroid | ditto | 
TrustDroid | ditto | 
FlaskDroid | mediate component interactions | 
SEAndroid | ditto | 
Aquifer | enforces information flow control policies that follow the user's UI workflow | 
IPC Inspection | track Android intent messages through a chain of applications to prevent privilege exscalation attacks | 
Quire | ditto | 
APEX | provide fine-grained permissions | 
CRePE | ditto | 
TISSA | allow fine-grained policies as well as allow the substitution of fake information into Android APIs - 1) | 
MockDroid | ditto | 
TaintDroid | dynamically track privacy sensitive informatino as it is used within an application - 2) | 
AppFence | 1) + 2) |  


### ASM Design

