# Principle of least privilege

From Wikipedia, the free encyclopedia

[Jump to navigation](https://en.wikipedia.org/wiki/Principle_of_least_privilege#mw-head)[Jump to search](https://en.wikipedia.org/wiki/Principle_of_least_privilege#searchInput)

Not to be confused with [Rule of least power](https://en.wikipedia.org/wiki/Rule_of_least_power).

| [![img](https://upload.wikimedia.org/wikipedia/en/thumb/9/99/Question_book-new.svg/50px-Question_book-new.svg.png)](https://en.wikipedia.org/wiki/File:Question_book-new.svg) | This article **needs additional citations for [verification](https://en.wikipedia.org/wiki/Wikipedia:Verifiability)**. Please help [improve this article](https://en.wikipedia.org/w/index.php?title=Principle_of_least_privilege&action=edit) by [adding citations to reliable sources](https://en.wikipedia.org/wiki/Help:Referencing_for_beginners). Unsourced material may be challenged and removed. *Find sources:* ["Principle of least privilege"](https://www.google.com/search?as_eq=wikipedia&q="Principle+of+least+privilege") – [news](https://www.google.com/search?tbm=nws&q="Principle+of+least+privilege"+-wikipedia&tbs=ar:1) **·** [newspapers](https://www.google.com/search?&q="Principle+of+least+privilege"&tbs=bkt:s&tbm=bks) **·** [books](https://www.google.com/search?tbs=bks:1&q="Principle+of+least+privilege"+-wikipedia) **·** [scholar](https://scholar.google.com/scholar?q="Principle+of+least+privilege") **·** [JSTOR](https://www.jstor.org/action/doBasicSearch?Query="Principle+of+least+privilege"&acc=on&wc=on) *(April 2019)* *([Learn how and when to remove this template message](https://en.wikipedia.org/wiki/Help:Maintenance_template_removal))* |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
|                                                              |                                                              |

In [information security](https://en.wikipedia.org/wiki/Information_security), [computer science](https://en.wikipedia.org/wiki/Computer_science), and other fields, the **principle of least privilege** (**PoLP**), also known as the **principle of minimal privilege** or the **principle of least authority**, requires that in a particular [abstraction layer](https://en.wikipedia.org/wiki/Abstraction_layer) of a computing environment, every module (such as a [process](https://en.wikipedia.org/wiki/Process_(computing)), a [user](https://en.wikipedia.org/wiki/User_(computing)), or a [program](https://en.wikipedia.org/wiki/Computer_program), depending on the subject) must be able to access only the information and [resources](https://en.wikipedia.org/wiki/Resource_(computer_science)) that are necessary for its legitimate purpose.[[1\]](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_note-1)

## Contents



- [1Details](https://en.wikipedia.org/wiki/Principle_of_least_privilege#Details)
- [2Implementation](https://en.wikipedia.org/wiki/Principle_of_least_privilege#Implementation)
- [3Similar principles](https://en.wikipedia.org/wiki/Principle_of_least_privilege#Similar_principles)
- [4See also](https://en.wikipedia.org/wiki/Principle_of_least_privilege#See_also)
- [5References](https://en.wikipedia.org/wiki/Principle_of_least_privilege#References)
- [6Bibliography](https://en.wikipedia.org/wiki/Principle_of_least_privilege#Bibliography)
- [7External links](https://en.wikipedia.org/wiki/Principle_of_least_privilege#External_links)

## Details[[edit](https://en.wikipedia.org/w/index.php?title=Principle_of_least_privilege&action=edit&section=1)]

The principle means giving a [user account](https://en.wikipedia.org/wiki/User_account) or process only those privileges which are essential to perform its intended function. For example, a user account for the sole purpose of creating backups does not need to install software: hence, it has rights only to run backup and backup-related applications. Any other privileges, such as installing new software, are blocked. The principle applies also to a personal computer user who usually does work in a normal user account, and opens a privileged, password protected account only when the situation absolutely demands it.

When applied to [users](https://en.wikipedia.org/wiki/User_(computing)), the terms *least user access* or *least-privileged user account* (LUA) are also used, referring to the concept that all [user accounts](https://en.wikipedia.org/wiki/User_account) should run with as few [privileges](https://en.wikipedia.org/wiki/Privilege_(computer_science)) as possible, and also launch [applications](https://en.wikipedia.org/wiki/Application_software) with as few privileges as possible.

The principle of least privilege is widely recognized as an important design consideration in enhancing the protection of data and functionality from faults ([fault tolerance](https://en.wikipedia.org/wiki/Fault_tolerance)) and malicious behavior ([computer security](https://en.wikipedia.org/wiki/Computer_security)).

Benefits of the principle include:

- Better system stability. When code is limited in the scope of changes it can make to a system, it is easier to test its possible actions and interactions with other applications. In practice for example, applications running with restricted rights will not have access to perform operations that could crash a machine, or adversely affect other applications running on the same system.
- Better system security. When code is limited in the system-wide actions it may perform, vulnerabilities in one application cannot be used to exploit the rest of the machine. For example, Microsoft states “Running in standard user mode gives customers increased protection against inadvertent system-level damage caused by "[shatter attacks](https://en.wikipedia.org/wiki/Shatter_attack)" and [malware](https://en.wikipedia.org/wiki/Malware), such as [root kits](https://en.wikipedia.org/wiki/Root_kit), [spyware](https://en.wikipedia.org/wiki/Spyware), and undetectable [viruses](https://en.wikipedia.org/wiki/Computer_virus)”.[[2\]](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_note-2)
- Ease of deployment. In general, the fewer privileges an application requires, the easier it is to deploy within a larger environment. This usually results from the first two benefits, applications that install device drivers or require elevated security privileges typically have additional steps involved in their deployment. For example, on Windows a solution with no [device drivers](https://en.wikipedia.org/wiki/Device_driver) can be run directly with no installation, while device drivers must be installed separately using the Windows installer service in order to grant the driver elevated privileges.[[3\]](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_note-3)

In practice, there exist multiple competing definitions of true least privilege. As [program complexity](https://en.wikipedia.org/wiki/Programming_complexity) increases rapidly, so do the number of potential issues, rendering a predictive approach impractical. Examples include the values of variables it may process, addresses it will need, or the precise time such things will be required. Object capability systems allow, for instance, deferring granting a single-use privilege until the time when it will be used. Currently, the closest practical approach is to eliminate privileges that can be manually evaluated as unnecessary. The resulting set of privileges typically exceeds the true minimum required privileges for the process.

Another limitation is the granularity of control that the operating environment has over privileges for an individual process.[[4\]](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_note-4) In practice, it is rarely possible to control a process's access to memory, processing time, I/O device addresses or modes with the precision needed to facilitate only the precise set of privileges a process will require.

The original formulation is from [Jerome Saltzer](https://en.wikipedia.org/wiki/Jerome_H._Saltzer):[[5\]](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_note-5)

> Every program and every privileged user of the system should operate using the least amount of privilege necessary to complete the job.
>
> — [Jerome Saltzer](https://en.wikipedia.org/wiki/Jerome_H._Saltzer), *[Communications of the ACM](https://en.wikipedia.org/wiki/Communications_of_the_ACM)*

[Peter J. Denning](https://en.wikipedia.org/wiki/Peter_J._Denning), in his paper "Fault Tolerant Operating Systems", set it in a broader perspective among four fundamental principles of fault tolerance.

Dynamic assignments of privileges was earlier discussed by [Roger Needham](https://en.wikipedia.org/wiki/Roger_Needham) in 1972.[[6\]](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_note-6)[[7\]](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_note-7)

Historically, the oldest instance of least privilege is probably the source code of *login.c*, which begins execution with [super-user](https://en.wikipedia.org/wiki/Super-user) permissions and—the instant they are no longer necessary—dismisses them via *setuid()* with a non-zero argument as demonstrated in the [Version 6 Unix](https://en.wikipedia.org/wiki/Version_6_Unix) [source code.](http://www.retro11.de/ouxr/u6ed/usr/source/s1/login.c.html#n:132)

## Implementation[[edit](https://en.wikipedia.org/w/index.php?title=Principle_of_least_privilege&action=edit&section=2)]

The [kernel](https://en.wikipedia.org/wiki/Kernel_(operating_system)) always runs with maximum privileges since it is the [operating system](https://en.wikipedia.org/wiki/Operating_system) core and has hardware access. One of the principal responsibilities of an operating system, particularly a multi-user operating system, is management of the hardware's availability and requests to access it from running [processes](https://en.wikipedia.org/wiki/Process_(computing)). When the kernel crashes, the mechanisms by which it maintains [state](https://en.wikipedia.org/wiki/State_(computer_science)#Program_state) also fail. Therefore, even if there is a way for the [CPU](https://en.wikipedia.org/wiki/Central_processing_unit) to recover without a [hard reset](https://en.wikipedia.org/wiki/Hard_reset), security continues to be enforced, but the operating system cannot properly respond to the failure because it was not possible to detect the failure. This is because kernel execution either halted or the [program counter](https://en.wikipedia.org/wiki/Program_counter) resumed execution from somewhere in an endless, and—usually—non-functional [loop](https://en.wikipedia.org/wiki/Control_flow#Loops).[*[citation needed](https://en.wikipedia.org/wiki/Wikipedia:Citation_needed)*] This would be akin to either experiencing [amnesia](https://en.wikipedia.org/wiki/Amnesia) (kernel execution failure) or being trapped in a closed maze that always returns to the starting point (closed loops).

[![img](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Priv_rings.svg/300px-Priv_rings.svg.png)](https://en.wikipedia.org/wiki/File:Priv_rings.svg)

The principle of least privilege demonstrated by privilege rings for the [Intel x86](https://en.wikipedia.org/wiki/Intel_x86)

If execution picks up after the crash by loading and running [trojan code](https://en.wikipedia.org/wiki/Trojan_horse_(computing)), the author of the trojan code can usurp control of all processes. The principle of least privilege forces code to run with the lowest privilege/permission level possible. This means that the code that resumes the code execution-whether trojan or simply code execution picking up from an unexpected location—would not have the ability to perform malicious or undesirable processes. One method used to accomplish this can be implemented in the [microprocessor](https://en.wikipedia.org/wiki/Microprocessor) hardware. For example, in the [Intel x86](https://en.wikipedia.org/wiki/Intel_x86) architecture the manufacturer designed four (ring 0 through ring 3) running "modes" with graduated degrees of access-much like [security clearance](https://en.wikipedia.org/wiki/Security_clearance) systems in defence and intelligence agencies.[*[citation needed](https://en.wikipedia.org/wiki/Wikipedia:Citation_needed)*]

As implemented in some operating systems, processes execute with a *potential privilege set* and an *active privilege set*.[*[citation needed](https://en.wikipedia.org/wiki/Wikipedia:Citation_needed)*] Such privilege sets are inherited from the parent as determined by the semantics of *[fork](https://en.wikipedia.org/wiki/Fork_(operating_system))()*. An [executable file](https://en.wikipedia.org/wiki/Executable_file) that performs a privileged function—thereby technically constituting a component of the [TCB](https://en.wikipedia.org/wiki/Trusted_computing_base), and concomitantly termed a trusted program or trusted process—may also be marked with a set of privileges. This is a logical extension of the notions of [set user ID](https://en.wikipedia.org/wiki/Setuid) and [set group ID](https://en.wikipedia.org/wiki/Setgid).[*[citation needed](https://en.wikipedia.org/wiki/Wikipedia:Citation_needed)*] The inheritance of [file privileges](https://en.wikipedia.org/wiki/File_privileges) by a process are determined by the semantics of the *[exec](https://en.wikipedia.org/wiki/Exec_(system_call))()* family of [system calls](https://en.wikipedia.org/wiki/System_calls). The precise manner in which potential process privileges, actual process privileges, and file privileges interact can become complex. In practice, least privilege is practiced by forcing a process to run with only those privileges required by the task. Adherence to this model is quite complex as well as error-prone.

## Similar principles[[edit](https://en.wikipedia.org/w/index.php?title=Principle_of_least_privilege&action=edit&section=3)]

The [Trusted Computer System Evaluation Criteria](https://en.wikipedia.org/wiki/Trusted_Computer_System_Evaluation_Criteria) (TCSEC) concept of [trusted computing base](https://en.wikipedia.org/wiki/Trusted_computing_base) (TCB) minimization is a far more stringent requirement that is only applicable to the functionally strongest assurance classes, *viz.*, B3 and A1 (which are *evidentiarily* different but *functionally* identical).

Least privilege is often associated with [privilege bracketing](https://en.wikipedia.org/wiki/Privilege_bracketing): that is, assuming necessary privileges at the last possible moment and dismissing them as soon as no longer strictly necessary, therefore ostensibly reducing fallout from erroneous code that unintentionally exploits more privilege than is merited. Least privilege has also been interpreted in the context of distribution of [discretionary access control](https://en.wikipedia.org/wiki/Discretionary_access_control) (DAC) permissions, for example asserting that giving user U read/write access to file F violates least privilege if U can complete his authorized tasks with only read permission.

## See also[[edit](https://en.wikipedia.org/w/index.php?title=Principle_of_least_privilege&action=edit&section=4)]

- [User Account Control](https://en.wikipedia.org/wiki/User_Account_Control)
- [Capability-based security](https://en.wikipedia.org/wiki/Capability-based_security)
- [Compartmentalization (intelligence)](https://en.wikipedia.org/wiki/Compartmentalization_(intelligence))
- [Confused deputy problem](https://en.wikipedia.org/wiki/Confused_deputy_problem)
- [Encapsulation (object-oriented programming)](https://en.wikipedia.org/wiki/Encapsulation_(object-oriented_programming))
- [Need to know](https://en.wikipedia.org/wiki/Need_to_know)
- [Privilege bracketing](https://en.wikipedia.org/wiki/Privilege_bracketing)
- [Privilege escalation](https://en.wikipedia.org/wiki/Privilege_escalation)
- [Privilege revocation (computing)](https://en.wikipedia.org/wiki/Privilege_revocation_(computing))
- [Privilege separation](https://en.wikipedia.org/wiki/Privilege_separation)
- [Protection ring](https://en.wikipedia.org/wiki/Protection_ring)
- [setuid](https://en.wikipedia.org/wiki/Setuid)
- [sudo](https://en.wikipedia.org/wiki/Sudo)

## References[[edit](https://en.wikipedia.org/w/index.php?title=Principle_of_least_privilege&action=edit&section=5)]

1. **[^](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_ref-1)** Saltzer & Schroeder 75
2. **[^](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_ref-2)** Jonathan, Clark; DABCC Inc. ["Virtualization Guru Writes "User-mode is a Good Thing - Deployment to Locked-down Accounts without Security Elevation""](http://www.dabcc.com/article.aspx?id=4135). Retrieved 15 Mar 2013.
3. **[^](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_ref-3)** Aaron Margosis (August 2006). ["Problems of Privilege: Find and Fix LUA Bugs"](https://technet.microsoft.com/en-us/magazine/cc160944.aspx). [Microsoft](https://en.wikipedia.org/wiki/Microsoft).
4. **[^](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_ref-4)** [Matt Bishop, *Computer Security: Art and Science*, Boston, MA: Addison-Wesley, 2003. pp. 343-344 cited Barnum & Gegick 2005](https://buildsecurityin.us-cert.gov/daisy/bsi/articles/knowledge/principles/351.html)
5. **[^](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_ref-5)** Saltzer, Jerome H. (1974). "Protection and the control of information sharing in multics". *[Communications of the ACM](https://en.wikipedia.org/wiki/Communications_of_the_ACM)*. **17** (7): 388–402. [CiteSeerX](https://en.wikipedia.org/wiki/CiteSeerX_(identifier)) [10.1.1.226.3939](https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.226.3939). [doi](https://en.wikipedia.org/wiki/Doi_(identifier)):[10.1145/361011.361067](https://doi.org/10.1145%2F361011.361067). [ISSN](https://en.wikipedia.org/wiki/ISSN_(identifier)) [0001-0782](https://www.worldcat.org/issn/0001-0782). [S2CID](https://en.wikipedia.org/wiki/S2CID_(identifier)) [326132](https://api.semanticscholar.org/CorpusID:326132).
6. **[^](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_ref-6)** Needham, R. M. (1972). "Protection systems and protection implementations". *Proceedings of the AFIPS '72 Fall Joint Computer Conference, December 5-7, 1972, Part I*. pp. 571–578. [doi](https://en.wikipedia.org/wiki/Doi_(identifier)):[10.1145/1479992.1480073](https://doi.org/10.1145%2F1479992.1480073). [S2CID](https://en.wikipedia.org/wiki/S2CID_(identifier)) [7371342](https://api.semanticscholar.org/CorpusID:7371342).
7. **[^](https://en.wikipedia.org/wiki/Principle_of_least_privilege#cite_ref-7)** Fred B. Schneider. ["Least Privilege and More"](http://www.cs.cornell.edu/fbs/publications/leastPrivNeedham.pdf) (PDF).

## Bibliography[[edit](https://en.wikipedia.org/w/index.php?title=Principle_of_least_privilege&action=edit&section=6)]

- Ben Mankin, *The Formalisation of Protection Systems*, Ph.D. thesis, University of Bath, 2004
- [P. J. Denning](https://en.wikipedia.org/wiki/P._J._Denning) (December 1976). "Fault tolerant operating systems". *[ACM Computing Surveys](https://en.wikipedia.org/wiki/ACM_Computing_Surveys)*. **8** (4): 359–389. [doi](https://en.wikipedia.org/wiki/Doi_(identifier)):[10.1145/356678.356680](https://doi.org/10.1145%2F356678.356680). [S2CID](https://en.wikipedia.org/wiki/S2CID_(identifier)) [207736773](https://api.semanticscholar.org/CorpusID:207736773).
- Jerry H. Saltzer, Mike D. Schroeder (September 1975). ["The protection of information in computer systems"](http://web.mit.edu/Saltzer/www/publications/protection/). *Proceedings of the IEEE*. **63** (9): 1278–1308. [CiteSeerX](https://en.wikipedia.org/wiki/CiteSeerX_(identifier)) [10.1.1.126.9257](https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.126.9257). [doi](https://en.wikipedia.org/wiki/Doi_(identifier)):[10.1109/PROC.1975.9939](https://doi.org/10.1109%2FPROC.1975.9939). [S2CID](https://en.wikipedia.org/wiki/S2CID_(identifier)) [269166](https://api.semanticscholar.org/CorpusID:269166).
- Deitel, Harvey M. (1990). [*An introduction to operating systems*](https://archive.org/details/introductiontoopdeit00deit/page/673) (revisited first ed.). Addison-Wesley. p. [673](https://archive.org/details/introductiontoopdeit00deit/page/673). [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier)) [978-0-201-14502-1](https://en.wikipedia.org/wiki/Special:BookSources/978-0-201-14502-1). page 31.
- Sean Martin (April 2012). ["Are security basics getting lost under the cover of cloud and mobile?"](http://www.scmagazine.com/are-security-basics-getting-lost-under-the-cover-of-cloud-and-mobile/article/236285/). *SC Magazine*.
- SANS Institute (May 2013). ["20 Critical Security Controls"](https://web.archive.org/web/20131101135802/http://www.sans.org/critical-security-controls/spring-2013-poster.pdf) (PDF). *SANS Institute*. Archived from [the original](http://www.sans.org/critical-security-controls/spring-2013-poster.pdf) (PDF) on 2013-11-01.

## External links[[edit](https://en.wikipedia.org/w/index.php?title=Principle_of_least_privilege&action=edit&section=7)]

- [Managing least privileges from the cloud by Monique Sendze](http://www.gsnmagazine.com/node/26227?c=cyber_security)
- [The Saltzer and Schroeder paper cited in the references.](http://web.mit.edu/Saltzer/www/publications/protection/)
- [NSA (the one that implemented SELinux) talks about the principle of least privilege](https://web.archive.org/web/20080228180840/http://cyberforge.com/weblog/aniltj/archive/2004/05/26/544.aspx)
- [A discussion of the implementation of the principle of least privilege in Solaris](http://www.sun.com/bigadmin/features/articles/least_privilege.html)
- [Tom's IT Pro: Most Organizations Unaware of Employees With Admin Rights](http://www.tomsitpro.com/articles/administrator_rights-admin_rights-malware-IT_security_professionals,1-353.html)
- ["Proof that LUA makes you safer" by Dana Epp](http://silverstr.ufies.org/blog/archives/000913.html)
- [Applying the Principle of Least Privilege to User Accounts on Windows XP, by Microsoft](https://technet.microsoft.com/en-us/library/bb456992.aspx)
- ["Commercial enterprises are putting our critical infrastructure at risk" CSO](http://www.csoonline.com/article/705800/commercial-enterprises-are-putting-our-critical-infrastructure-at-risk?page=1)
- [How to successfully implement the principle of least privilege](https://www.techrepublic.com/blog/it-security/how-to-successfully-implement-the-principle-of-least-privilege/)

| hide[v](https://en.wikipedia.org/wiki/Template:Object-capability_security)[t](https://en.wikipedia.org/wiki/Template_talk:Object-capability_security)[e](https://en.wikipedia.org/w/index.php?title=Template:Object-capability_security&action=edit)[Object-capability](https://en.wikipedia.org/wiki/Object-capability_model) security |                                                              |
| -----------------------------------------------------------: | ------------------------------------------------------------ |
|                                                     Concepts | Principle of least privilege (PoLP)[Confused deputy problem](https://en.wikipedia.org/wiki/Confused_deputy_problem)[Ambient authority](https://en.wikipedia.org/wiki/Ambient_authority)[File descriptor](https://en.wikipedia.org/wiki/File_descriptor)[C-list](https://en.wikipedia.org/wiki/C-list_(computer_security))[Object-capability model](https://en.wikipedia.org/wiki/Object-capability_model)[Capability-based security](https://en.wikipedia.org/wiki/Capability-based_security)[Capability-based addressing](https://en.wikipedia.org/wiki/Capability-based_addressing)[Zooko's triangle](https://en.wikipedia.org/wiki/Zooko's_triangle)[Petnames](https://en.wikipedia.org/wiki/Petname) |
| [Operating systems](https://en.wikipedia.org/wiki/Operating_system), [kernels](https://en.wikipedia.org/wiki/Kernel_(operating_system)) | [Capsicum](https://en.wikipedia.org/wiki/Capsicum_(Unix))[Fuchsia](https://en.wikipedia.org/wiki/Fuchsia_(operating_system))[Genode](https://en.wikipedia.org/wiki/Genode)[GNOSIS](https://en.wikipedia.org/wiki/GNOSIS) → [KeyKOS](https://en.wikipedia.org/wiki/KeyKOS) → [EROS](https://en.wikipedia.org/wiki/EROS_(microkernel)) → [CapROS](https://en.wikipedia.org/wiki/CapROS)[Hydra](https://en.wikipedia.org/wiki/Hydra_(operating_system))[iMAX 432](https://en.wikipedia.org/wiki/IMAX_432)[Midori](https://en.wikipedia.org/wiki/Midori_(operating_system))[NLTSS](https://en.wikipedia.org/wiki/NLTSS)[seL4](https://en.wikipedia.org/wiki/L4_microkernel_family#High_assurance:_seL4) |
| [Programming languages](https://en.wikipedia.org/wiki/Programming_language) | [Cajita](https://en.wikipedia.org/wiki/Caja_project)[E](https://en.wikipedia.org/wiki/E_(programming_language))[Joe-E](https://en.wikipedia.org/wiki/Joe-E)[Joule](https://en.wikipedia.org/wiki/Joule_(programming_language)) |
|    [File systems](https://en.wikipedia.org/wiki/File_system) | [Tahoe-LAFS](https://en.wikipedia.org/wiki/Tahoe-LAFS)       |
|                                         Specialised hardware | [BiiN](https://en.wikipedia.org/wiki/BiiN)[Cambridge CAP](https://en.wikipedia.org/wiki/CAP_computer)[Flex](https://en.wikipedia.org/wiki/Flex_machine)[IBM System/38](https://en.wikipedia.org/wiki/IBM_System/38)[Intel iAPX 432](https://en.wikipedia.org/wiki/Intel_iAPX_432)[Plessey System 250](https://en.wikipedia.org/wiki/Plessey_System_250) |

[Categories](https://en.wikipedia.org/wiki/Help:Category): 

- [Information theory](https://en.wikipedia.org/wiki/Category:Information_theory)
- [Computer security](https://en.wikipedia.org/wiki/Category:Computer_security)