---
title: "Talks and abstracts"
date: 2016-09-17
draft: false
featured_image: "/images/bsides_logo_blue.jpg"
featured_image_desc: "BSides Zurich logo"
---

## Keynote

{{< figure src="/archives/2016/keynote.jpg" height="300px" class="img-center mt0 fl" >}}

Max Moser ([@rexploit](https://twitter.com/rexploit)) has worked for many years
in the field of IT-Security. He has supported many national and international
companies, public authorities and institutions to analyze and improve their
security levels. He specializes in protocol analysis, research and highly
specific penetration testing of complex environments. Max Moser is known within
the IT-Security arena for his open-source projects such as the Linux
distribution BackTrack as well as the recent Keykeriki research project. For
years, he has made available both projects as well as other security-relevant
information for the interested public (<http://www.remote-exploit.org>). Within
the limits of their own business activity, security professionals worldwide
apply this information and these products. The imparting of knowledge tailored
workshops with a strong practical element is one of his great passions. Max
Moser supports companies and corporations from various market sectors including
telecommunications, pharmaceuticals, Insurance and banking. He presented several
research project results at well-known international security conferences such
as Black Hat, CanSecWest, etc., and his expertise is well represented in
national and international media.

### How to defend from an attacker armed with a mathematician [Slides](/archives/2016/ASanso-bsides.pdf)

*Antonio Sanso ([@asanso](https://twitter.com/asanso))*

Diffie-Hellman key exchange is one of the most common public-key cryptographic
methods in use in the Internet. It is a fundamental building block for IPsec,
SSH, and TLS. Diffie-Hellman key exchange allows two parties to agree on a
shared secret in the presence of an eavesdropper. Since the security of
Diffie-Hellman relies crucially on the group parameters, implementations can be
vulnerable to an attacker who provides maliciously generated parameters that
change the properties of the group. In January 2016 we found a vulnerability
affecting OpenSSL leveraging indeed this kind of attack (CVE-2016-0701). The
research made while studying OpenSSL code base also highlighted a
semi-mysterious RFC (RFC 5114 – “Additional Dif e-Hellman Groups for Use with
IETF Standards”) originating from Defense contractor BBN. The mathematical
property of the groups introduced in RFC 5114 were of particular interest since
made OpenSSL particularly susceptible OpenSSL to a Key Recovery Attack.

### Reporting the Kill Chain [Slides](/archives/2016/bsideszh2016_svetsch_reporting_the_kill_chain.pdf)

*Sven Vetsch ([@disenchant](https://twitter.com/disenchant))*

Everyone in the technical security industry has to do it, everyone hates it –
reporting. If you’re for example a penetration tester and you’ve identified a
missing patch on a target, reporting is quite easy: “Patch X is missing on
target Y but you should totally install it because of vulnerability Z”. Today
our industry is facing way more complex situation, be it in incident response,
attack forensics, red teaming or even threat modelling. When you’re trying to
explain an attack to a client, this can be done by using a step by step approach
but lets be honest, normally there’s not just one straight line from the
attacker to the final target. Most often we find ourselves in a situation, where
our work looks more like a rather complex graph that we traversed in multiple
ways during an assignment. Unfortunately, a bunch of sequentially ordered papers
is very bad for representing something that is really a graph and it’s therefore
an insufficient deliverable to hand over to a client. So do we have to find a
new form to deliver reports? Should we change our approach on analyzing and
performing attacks so they can still be put on paper? Can visualization help us
explaining what we’ve done and why? In this presentation I won’t be able to
provide you with any answers for those questions. What I can do, is showing you
some different ways of how my colleagues and I at Redguard have tried to
approach those questions and what kind of dead-ends we hit. If everything goes
well, I can share our pain with the audience and in the discussion groups we
would then see what others tried and who knows, maybe together we find the
magical unicorn of reporting formats.

### Indicators of compromise – wasting resources, revealing too much or following false flags?

*Candid Wüest ([@mylaocoon](https://twitter.com/mylaocoon))*

Sharing indicators of compromise (IOC) is commonly used to fight against APTs;
however, irrespective of how fast they are obtained or how many are available
they are steadily losing their value. Advanced attackers have long ago changed
their methods and tactics – where necessary. They are using unique C&C servers
and freshly compiled malware for each target which renders the sharing of most
IOCs useless; with very little effort on behalf of the attacker. On the other
hand, sharing such IOCs publicly can reveal the researchers knowledge about the
attack to everyone. Attackers can learn if their campaign have been uncovered
and sometimes even how they can improve their broken attack code. Should we not
publish data at all then? Furthermore, how can you be sure that the attackers
did not deliberately plant a le which would lead you to believe that the
culprits were… (*rolling attribution dice*)… the Chinese? How can you be sure
that you are not mixing IOCs from multiple attack groups which all have
compromised your servers? This talk will try and explain where IOCs might still
be useful and how they can be combined with other threat intelligence data to be
more reliable. Supported by real world examples and statistics from our own
analysis of current attacks we will illustrate various cases and discuss strange
artifacts that we have seen.

### Advanced Detection using Sysmon [Slides](/archives/2016/Sysmon_BSidesZH_2016-09-17_PUBLIC.pdf)

*Tom Ueltschi ([@c_APT_ure](https://twitter.com/c_APT_ure))*

Enterprises and organizations of all sizes are struggling to prevent and detect
all malware attacks and advanced adversary actions inside their networks in a
timely manner. Prevention focused technology hasn’t been good enough to prevent
breaches for years and detection has been lacking in many ways. This
presentation will give an overview and detailed examples on how to use the free
Sysinternals tool SYSMON to greatly improve host-based incident detection and
enable threat hunting approaches. Splunk is just an example of a SIEM to
centralize Sysmon log data and be able to search and correlate large amounts of
data to create high-quality alerts with low false-positive rates. The same could
likely be done using another free or commercial SIEM. The main goal is to share
an approach, a methodology how to greatly improve host-based detection by using
Sysmon and Splunk to create alerts. One main topic throughout the presentation
will be how to nd suspicious or malicious behaviors, how to implement search
queries and how to reduce or eliminate false-positives. Examples will cover
different crimeware malware families as well as tools and TTPs used by Red Teams
and advanced adversaries. For the latter, a commercial tool (Cobalt Strike) was
used to test different privilege escalation and lateral movement techniques and
develop queries for detection. Sysinternals Process Monitor and Sysmon tools
were used to analyze behaviors on the endpoints involved. Any Blue Team member
should be able to take away some ideas and approaches to improve detection and
incident response readiness in their organization.

### badGPO – Using GPOs for Persistence and Lateral Movement [Slides](/archives/2016/160917_BSidesZH_badGPO_Kraft-Willi.pdf)

*Yves Kraft ([@nrx_ch](https://twitter.com/nrx_ch)), Immanuel Willi*

Group Policy is a feature which provides centralized management and
configuration functions for the Microsoft operating system, application and user
settings. Group Policy is simply the easiest way to reach out and configure
computer and user settings on networks based on Active Directory Domain Services
(AD DS). Such policies are widely used in enterprise environments to control
settings of clients and servers: registry settings, security options, scripts,
folders, and software installation and maintenance, just to name a few. Settings
are contained in so-called Group Policy Objects (GPOs) and can be misused in a
sneaky way to distribute malware and gain persistence in an automated manner in
a post exploitation scenario of an already compromised domain. In a proof of
concept, inspired by Phineas Fishers’ article about pwning HackingTeam, we will
show how persistence and lateral movement in a compromised company network can
be achieved, and demonstrate some PowershellEmpire Framework modules which we
created. PowershellEmpire is basically a post-exploitation framework that
utilises the widely-deployed PowerShell tool for all your system-smashing needs.
There are already functionalities built-in regarding GPOs. We tried to further
evolve the miss-use of GPOs in additional scenarios. Furthermore, we will
discuss some countermeasures including detection and prevention mechanisms.

### DNS-based threat hunting: learn, share and improve. repeat. [Slides](/archives/2016/bsideszh2016-dns-slides-final-joao.pdf)

*Joao Collier de Mendonca ([@sec_joao](https://twitter.com/sec_joao))*

DNS is one of the most important support services of IP-based networks: it is
essential a vast amount services and applications, from surfing the web to
connecting to a domain-controller or database server. From the defensive
perspective, DNS provides a clear overview/snapshot of your network activities.
The drawbacks of applying DNS-based analysis are the amount of data generated
and that often there is no clear starting point (traffic baseline) to enable
detection of anomalies and malicious activities. This talk aims at providing a
solid starting point to incident responders and security analysis on how to
leverage DNS-based analysis to quickly find out the most eminent threats in the
shortest time possible. It is also structured to enable discussion and
information exchange, supporting the development of further detections patterns
and methods.
