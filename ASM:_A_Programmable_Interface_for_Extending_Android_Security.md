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
[Kirin](http://delivery.acm.org/10.1145/1660000/1653691/p235-enck.pdf?ip=147.46.246.166&id=1653691&acc=ACTIVE%20SERVICE&key=0EC22F8658578FE1%2ED83A6478590749B7%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&CFID=519539945&CFTOKEN=32700454&__acm__=1406683501_5248a6caf3f197167328090a87a95565) | place constraints on permissions of applications being installed | O 
[Saint](http://www.enck.org/pubs/acsac09.pdf) | mediate communication between components in different applications | 
[XManDroid](http://www-infsec.cs.uni-saarland.de/~bugiel/publications/pdfs/XManDroid-tr-2011-04.pdf) | ditto | 
[TrustDroid](https://www.informatik.tu-darmstadt.de/fileadmin/user_upload/Group_TRUST/PubsPDF/spsm18-bugiel.pdf) | ditto | 
[FlaskDroid](https://www.informatik.tu-darmstadt.de/fileadmin/user_upload/Group_TRUST/PubsPDF/flaskdroid.pdf) | mediate component interactions | 
[SEAndroid](http://www.cs.columbia.edu/~lierranli/coms6998-7Spring2014/papers/SEAndroid-NDSS2013.pdf) | ditto | 
[Aquifer](http://www.enck.org/pubs/nadkarni-ccs13.pdf) | enforces information flow control policies that follow the user's UI workflow | 
[IPC Inspection]() | track Android intent messages through a chain of applications to prevent privilege exscalation attacks | 
[Quire](https://www.usenix.org/legacy/event/sec11/tech/full_papers/Dietz7-26-11.pdf) | ditto | 
[APEX](dl.acm.org/ft_gateway.cfm?id=1755732) | provide fine-grained permissions | 
[CRePE](http://dl.acm.org/citation.cfm?id=1949355) | ditto | 
[TISSA](http://www.cs.ncsu.edu/faculty/jiang/pubs/TRUST11.pdf) | allow fine-grained policies as well as allow the substitution of fake information into Android APIs - 1) | 
[MockDroid](http://www.cl.cam.ac.uk/~acr31/pubs/beresford-mockdroid.pdf) | ditto | 
[TaintDroid](http://static.usenix.org/event/osdi10/tech/full_papers/Enck.pdf) | dynamically track privacy sensitive informatino as it is used within an application - 2) | 
[AppFence](http://delivery.acm.org/10.1145/2050000/2046780/p639-hornyack.pdf?ip=147.46.246.166&id=2046780&acc=ACTIVE%20SERVICE&key=0EC22F8658578FE1%2ED83A6478590749B7%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&CFID=519200755&CFTOKEN=86906882&__acm__=1406621173_c5da226c79dd66cbadf9abcceaa90890) | 1) + 2) |  


### ASM Design

