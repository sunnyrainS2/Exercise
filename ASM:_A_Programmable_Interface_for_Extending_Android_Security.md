# ASM: A Programmable Interface for Extending Android Security.
Nadkarni, Adwait, and William Enck. 2014.

### Goal and contributions

##### Goal
> promote OS security extensibility in the Android platform

##### Contributions
> 1. identify the authorization hook semantics required for new operating systems such as Android.
> 2. design and implement the extensible Android Security Modules (ASM) framework.
> 3. implement two example ASM apps to demonstrate the utility of the ASM framework.


### Background
Android defines four types of components: *activity*, *service*, *broadcast receiver*, and *content provider*.


### Design Goals

> 1. Generic authorization expressibility
> 2. Ensure existing security quarantees
> 3. Protect kernel integrity
> 4. Multiple authorization modules
> 5. Minimize resource overhead


### Android security enhancements

System | security enhancements | Open
------ | --------------------- | ----
[Kirin](http://dl.acm.org/citation.cfm?id=1653691) | place constraints on permissions of applications being installed | O 
[Saint](http://www.enck.org/pubs/acsac09.pdf) | mediate communication between components in different applications | 
[XManDroid](http://www-infsec.cs.uni-saarland.de/~bugiel/publications/pdfs/XManDroid-tr-2011-04.pdf) | ditto | 
[TrustDroid](https://www.informatik.tu-darmstadt.de/fileadmin/user_upload/Group_TRUST/PubsPDF/spsm18-bugiel.pdf) | ditto | 
[FlaskDroid](https://www.informatik.tu-darmstadt.de/fileadmin/user_upload/Group_TRUST/PubsPDF/flaskdroid.pdf) | mediate component interactions | 
[SEAndroid](http://www.cs.columbia.edu/~lierranli/coms6998-7Spring2014/papers/SEAndroid-NDSS2013.pdf) | ditto | 
[Aquifer](http://www.enck.org/pubs/nadkarni-ccs13.pdf) | enforces information flow control policies that follow the user's UI workflow | 
[IPC Inspection]() | track Android intent messages through a chain of applications to prevent privilege exscalation attacks | 
[Quire](https://www.usenix.org/legacy/event/sec11/tech/full_papers/Dietz7-26-11.pdf) | ditto | 
[APEX](http://dl.acm.org/citation.cfm?id=1755732) | provide fine-grained permissions | 
[CRePE](http://dl.acm.org/citation.cfm?id=1949355) | ditto | 
[TISSA](http://www.cs.ncsu.edu/faculty/jiang/pubs/TRUST11.pdf) | allow fine-grained policies as well as allow the substitution of fake information into Android APIs - 1) | 
[MockDroid](http://www.cl.cam.ac.uk/~acr31/pubs/beresford-mockdroid.pdf) | ditto | 
[TaintDroid](http://static.usenix.org/event/osdi10/tech/full_papers/Enck.pdf) | dynamically track privacy sensitive informatino as it is used within an application - 2) | 
[AppFence](http://dl.acm.org/citation.cfm?id=2046780) | 1) + 2) |  


### ASM Design

