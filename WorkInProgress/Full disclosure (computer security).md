# Full disclosure (computer security)

From Wikipedia, the free encyclopedia

[Jump to navigation](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#mw-head)[Jump to search](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#searchInput)

This article is about vulnerability disclosure. For other uses, see [Full disclosure (disambiguation)](https://en.wikipedia.org/wiki/Full_disclosure_(disambiguation)).

In the field of [computer security](https://en.wikipedia.org/wiki/Computer_security), independent researchers often discover flaws in software that can be abused to cause unintended behaviour; these flaws are called [vulnerabilities](https://en.wikipedia.org/wiki/Vulnerability_(computing)). The process by which the analysis of these vulnerabilities is shared with third parties is the subject of much debate, and is referred to as the researcher's *disclosure policy*. **Full disclosure** is the practice of publishing analysis of software vulnerabilities as early as possible, making the data accessible to everyone without restriction. The primary purpose of widely disseminating information about vulnerabilities is so that potential victims are as knowledgeable as those who attack them.[[1\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-exposing-1)

In his 2007 essay on the topic, [Bruce Schneier](https://en.wikipedia.org/wiki/Bruce_Schneier) stated "Full disclosure – the practice of making the details of security vulnerabilities public – is a damned good idea. Public scrutiny is the only reliable way to improve security, while secrecy only makes us less secure".[[2\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-schneier-2) [Leonard Rose](https://en.wikipedia.org/wiki/Leonard_Rose_(hacker)), co-creator of an [electronic mailing list](https://en.wikipedia.org/wiki/Electronic_mailing_list) that has superseded [bugtraq](https://en.wikipedia.org/wiki/Bugtraq) to become the de facto forum for disseminating advisories, explains "We don't believe in security by obscurity, and as far as we know, full disclosure is the only way to ensure that everyone, not just the insiders, have access to the information we need."[[3\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-fulldisc-3)

## Contents



- 1The vulnerability disclosure debate
  - [1.1Coordinated vulnerability disclosure](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#Coordinated_vulnerability_disclosure)
  - [1.2Full disclosure](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#Full_disclosure)
  - [1.3Non disclosure](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#Non_disclosure)
  - 1.4Debate
    - [1.4.1Arguments against coordinated disclosure](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#Arguments_against_coordinated_disclosure)
    - [1.4.2Arguments against non disclosure](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#Arguments_against_non_disclosure)
- [2References](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#References)

## The vulnerability disclosure debate[[edit](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=edit&section=1)]

The controversy around the public disclosure of sensitive information is not new. The issue of full disclosure was first raised in the context of locksmithing, in a 19th-century controversy regarding whether weaknesses in lock systems should be kept secret in the locksmithing community, or revealed to the public.[[4\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-hobbs-4) Today, there are three major disclosure policies under which most others can be categorized:[[5\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-sans-5) [Non Disclosure](https://en.wikipedia.org/wiki/Non-disclosure_agreement), [Coordinated Disclosure](https://en.wikipedia.org/wiki/Responsible_disclosure), and Full Disclosure.

The major stakeholders in vulnerability research have their disclosure policies shaped by various motivations, it is not uncommon to observe campaigning, marketing or lobbying for their preferred policy to be adopted and chastising those who dissent. Many prominent security researchers favor full disclosure, whereas most vendors prefer coordinated disclosure. Non disclosure is generally favored by commercial exploit vendors and [blackhat hackers](https://en.wikipedia.org/wiki/Hacker_(computer_security)#Black_hat).[[6\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-Moore2005-6)

### Coordinated vulnerability disclosure[[edit](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=edit&section=2)]

Coordinated vulnerability disclosure is a policy under which researchers agree to report vulnerabilities to a coordinating authority, which then reports it to the vendor, tracks fixes and mitigations, and coordinates the disclosure of information with stakeholders including the public.[[7\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-7) In some cases the coordinating authority is the vendor. The premise of coordinated disclosure is typically that nobody should be informed about a vulnerability until the software vendor says it is time.[[8\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-8)[[9\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-rfc-9) While there are often exceptions or variations of this policy, distribution must initially be limited and vendors are given privileged access to nonpublic research.

The original name for this approach was “[responsible disclosure](https://en.wikipedia.org/wiki/Responsible_disclosure)”, based on the essay by Microsoft Security Manager Scott Culp “It's Time to End Information Anarchy”[[10\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-culp-10) (referring to full disclosure). Microsoft later called for the term to be phased out in favor of “Coordinated Vulnerability Disclosure” (CVD).[[11\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-co-ord-11)[[12\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-mssec-12)

Although the reasoning varies, many practitioners argue that end-users cannot benefit from access to vulnerability information without guidance or patches from the vendor, so the risks of sharing research with malicious actors is too great for too little benefit. As Microsoft explain, "[Coordinated disclosure] serves everyone's best interests by ensuring that customers receive comprehensive, high-quality updates for security vulnerabilities but are not exposed to malicious attacks while the update is being developed."[[12\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-mssec-12)

### Full disclosure[[edit](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=edit&section=3)]

Full disclosure is the policy of publishing information on vulnerabilities without restriction as early as possible, making the information accessible to the general public without restriction. In general, proponents of full disclosure believe that the benefits of freely available vulnerability research outweigh the risks, whereas opponents prefer to limit the distribution.

The free availability of vulnerability information allows users and administrators to understand and react to vulnerabilities in their systems, and allows customers to pressure vendors to fix vulnerabilities that vendors may otherwise feel no incentive to solve. There are some fundamental problems with coordinated disclosure that full disclosure can resolve.

- If customers do not know about vulnerabilities, they cannot request patches, and vendors experience no economic incentive to correct vulnerabilities.
- Administrators cannot make informed decisions about the risks to their systems, as information on vulnerabilities is restricted.
- Malicious researchers who also know about the flaw have a long period of time to continue exploiting the flaw.

Discovery of a specific flaw or vulnerability is not a mutually exclusive event, multiple researchers with differing motivations can and do discover the same flaws independently.

There is no standard way to make vulnerability information available to the public, researchers often use mailing lists dedicated to the topic, academic papers or industry conferences.

### Non disclosure[[edit](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=edit&section=4)]

Non disclosure is the policy that vulnerability information should not be shared, or should only be shared under non-disclosure agreement (either contractually or informally).

Common proponents of non-disclosure include commercial exploit vendors, researchers who intend to exploit the flaws they find,[[5\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-sans-5) and proponents of [security through obscurity](https://en.wikipedia.org/wiki/Security_through_obscurity).

### Debate[[edit](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=edit&section=5)]

#### Arguments against coordinated disclosure[[edit](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=edit&section=6)]

Researchers in favor of coordinated disclosure believe that users cannot make use of advanced knowledge of vulnerabilities without guidance from the vendor, and that the majority is best served by limiting distribution of vulnerability information. Advocates argue that low-skilled attackers can use this information to perform sophisticated attacks that would otherwise be beyond their ability, and the potential benefit does not outweigh the potential harm caused by malevolent actors. Only when the vendor has prepared guidance that even the most unsophisticated users can digest should the information be made public.

This argument presupposes that vulnerability discovery is a mutually exclusive event, that only one person can discover a vulnerability. There are many examples of vulnerabilities being discovered simultaneously, often being exploited in secrecy before discovery by other researchers.[[13\]](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_note-ac1d-13) While there may exist users who cannot benefit from vulnerability information, full disclosure advocates believe this demonstrates a contempt for the intelligence of end users. While it's true that some users cannot benefit from vulnerability information, if they're concerned with the security of their networks they are in a position to hire an expert to assist them as you would hire a mechanic to help with a car.

#### Arguments against non disclosure[[edit](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=edit&section=7)]

Non disclosure is typically used when a researcher intends to use knowledge of a vulnerability to attack computer systems operated by their enemies, or to trade knowledge of a vulnerability to a third party for profit, who will typically use it to attack their enemies.

Researchers practicing non disclosure are generally not concerned with improving security or protecting networks. However, some proponents argue that they simply do not want to assist vendors, and claim no intent to harm others.

While full and coordinated disclosure advocates declare similar goals and motivations, simply disagreeing on how best to achieve them, non disclosure is entirely incompatible.

## References[[edit](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=edit&section=8)]

1. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-exposing_1-0)** Heiser, Jay (January 2001). ["Exposing Infosecurity Hype"](https://web.archive.org/web/20060328012516/http://infosecuritymag.techtarget.com/articles/january01/columns_curmudgeons_corner.shtml). *Information Security Mag*. TechTarget. Archived from [the original](http://infosecuritymag.techtarget.com/articles/january01/columns_curmudgeons_corner.shtml) on 28 March 2006. Retrieved 29 April 2013.
2. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-schneier_2-0)** Schneier, Bruce (January 2007). ["Damned Good Idea"](https://www.schneier.com/essay-146.html). CSO Online. Retrieved 29 April 2013.
3. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-fulldisc_3-0)** Rose, Leonard. ["Full-Disclosure"](https://wayback.archive-it.org/all/20101223024433/https://lists.grok.org.uk/mailman/listinfo/full-disclosure). *A lightly-moderated mailing list for the discussion of security issues*. Archived from [the original](https://lists.grok.org.uk/mailman/listinfo/full-disclosure) on 23 December 2010. Retrieved 29 April 2013.
4. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-hobbs_4-0)** Hobbs, Alfred (1853). Locks and Safes: The Construction of Locks*. London: Virtue & Co.*
5. ^ [Jump up to:***a***](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-sans_5-0) [***b***](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-sans_5-1) Shepherd, Stephen. ["Vulnerability Disclosure: How do we define Responsible Disclosure?"](https://www.sans.org/reading_room/whitepapers/threats/define-responsible-disclosure_932). *SANS GIAC SEC PRACTICAL VER. 1.4B (OPTION 1)*. SANS Institute. Retrieved 29 April 2013.
6. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-Moore2005_6-0)** Moore, Robert (2005). *Cybercrime: Investigating High Technology Computer Crime*. Matthew Bender & Company. p. 258. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier)) [1-59345-303-5](https://en.wikipedia.org/wiki/Special:BookSources/1-59345-303-5).
7. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-7)** ["Software Vulnerability Disclosure in Europe"](https://www.ceps.eu/ceps-publications/software-vulnerability-disclosure-europe-technology-policies-and-legal-challenges/). *CEPS*. 2018-06-27. Retrieved 2019-10-18.
8. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-8)** ["Project Zero: Vulnerability Disclosure FAQ"](https://googleprojectzero.blogspot.com/p/vulnerability-disclosure-faq.html). *Project Zero*. Retrieved 2019-10-18.
9. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-rfc_9-0)** Christey, Steve. ["Responsible Vulnerability Disclosure Process"](https://tools.ietf.org/html/draft-christey-wysopal-vuln-disclosure-00). IETF. p. 3.3.2. Retrieved 29 April 2013.
10. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-culp_10-0)** Culp, Scott. ["It's Time to End Information Anarchy"](https://web.archive.org/web/20011109045330/http://www.microsoft.com/technet/treeview/default.asp?url=%2Ftechnet%2Fcolumns%2Fsecurity%2Fnoarch.asp). *Technet Security*. Microsoft TechNet. Archived from [the original](http://www.microsoft.com/technet/treeview/default.asp?url=/technet/columns/security/noarch.asp) on November 9, 2001. Retrieved 29 April 2013.
11. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-co-ord_11-0)** Goodin, Dan. ["Microsoft imposes security disclosure policy on all workers"](https://www.theregister.co.uk/2011/04/19/microsoft_vulnerability_disclosure_policy/print.html). *The Register*. Retrieved 29 April 2013.
12. ^ [Jump up to:***a***](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-mssec_12-0) [***b***](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-mssec_12-1) Microsoft Security. ["Coordinated Vulnerability Disclosure"](https://www.microsoft.com/security/msrc/report/disclosure.aspx). [Archived](https://web.archive.org/web/20141216085920/http://download.microsoft.com/download/2/5/5/255EF667-218D-42B1-84B4-1A21F39BA167/CVD.docx) from the original on 2014-12-16. Retrieved 29 April 2013.
13. **[^](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security)#cite_ref-ac1d_13-0)** B1tch3z, Ac1d. ["Ac1db1tch3z vs x86_64 Linux Kernel"](http://seclists.org/fulldisclosure/2010/Sep/268). Retrieved 29 April 2013.

[Categories](https://en.wikipedia.org/wiki/Help:Category): 

- [Computer security procedures](https://en.wikipedia.org/wiki/Category:Computer_security_procedures)

## Navigation menu

- Not logged in
- [Talk](https://en.wikipedia.org/wiki/Special:MyTalk)
- [Contributions](https://en.wikipedia.org/wiki/Special:MyContributions)
- [Create account](https://en.wikipedia.org/w/index.php?title=Special:CreateAccount&returnto=Full+disclosure+(computer+security))
- [Log in](https://en.wikipedia.org/w/index.php?title=Special:UserLogin&returnto=Full+disclosure+(computer+security))

- [Article](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security))
- [Talk](https://en.wikipedia.org/wiki/Talk:Full_disclosure_(computer_security))

- [Read](https://en.wikipedia.org/wiki/Full_disclosure_(computer_security))
- [Edit](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=edit)
- [View history](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=history)

### Search

- [Main page](https://en.wikipedia.org/wiki/Main_Page)
- [Contents](https://en.wikipedia.org/wiki/Wikipedia:Contents)
- [Current events](https://en.wikipedia.org/wiki/Portal:Current_events)
- [Random article](https://en.wikipedia.org/wiki/Special:Random)
- [About Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:About)
- [Contact us](https://en.wikipedia.org/wiki/Wikipedia:Contact_us)
- [Donate](https://donate.wikimedia.org/wiki/Special:FundraiserRedirector?utm_source=donate&utm_medium=sidebar&utm_campaign=C13_en.wikipedia.org&uselang=en)

### Contribute

- [Help](https://en.wikipedia.org/wiki/Help:Contents)
- [Learn to edit](https://en.wikipedia.org/wiki/Help:Introduction)
- [Community portal](https://en.wikipedia.org/wiki/Wikipedia:Community_portal)
- [Recent changes](https://en.wikipedia.org/wiki/Special:RecentChanges)
- [Upload file](https://en.wikipedia.org/wiki/Wikipedia:File_Upload_Wizard)

### Tools

- [What links here](https://en.wikipedia.org/wiki/Special:WhatLinksHere/Full_disclosure_(computer_security))
- [Related changes](https://en.wikipedia.org/wiki/Special:RecentChangesLinked/Full_disclosure_(computer_security))
- [Special pages](https://en.wikipedia.org/wiki/Special:SpecialPages)
- [Permanent link](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&oldid=1013071881)
- [Page information](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&action=info)
- [Cite this page](https://en.wikipedia.org/w/index.php?title=Special:CiteThisPage&page=Full_disclosure_(computer_security)&id=1013071881&wpFormIdentifier=titleform)
- [Wikidata item](https://www.wikidata.org/wiki/Special:EntityPage/Q842234)

### Print/export

- [Download as PDF](https://en.wikipedia.org/w/index.php?title=Special:DownloadAsPdf&page=Full_disclosure_(computer_security)&action=show-download-screen)
- [Printable version](https://en.wikipedia.org/w/index.php?title=Full_disclosure_(computer_security)&printable=yes)



### Languages

- [Čeština](https://cs.wikipedia.org/wiki/Full_disclosure)
- [Deutsch](https://de.wikipedia.org/wiki/Full_Disclosure_(IT-Sicherheit))
- [Español](https://es.wikipedia.org/wiki/Revelación_completa)
- [Français](https://fr.wikipedia.org/wiki/Divulgation_complète)
- [Italiano](https://it.wikipedia.org/wiki/Divulgazione_totale)
- [Magyar](https://hu.wikipedia.org/wiki/Teljes_közzététel)
- [日本語](https://ja.wikipedia.org/wiki/フルディスクロージャ)
- [Polski](https://pl.wikipedia.org/wiki/Full_disclosure)
- [Русский](https://ru.wikipedia.org/wiki/Полное_раскрытие)

[Edit links](https://www.wikidata.org/wiki/Special:EntityPage/Q842234#sitelinks-wikipedia)

- This page was last edited on 19 March 2021, at 21:31 (UTC).