---
title: "Talks and abstracts"
date: 2017-09-23
draft: false
featured_image: "/images/bsides_logo_blue.jpg"
featured_image_desc: "BSides Zurich logo"
---

## Keynote

{{< figure src="/archives/2017/keynote.png" height="300px" class="img-center mt0 fl" >}}

**Thomas Dullien / Halvar Flake**
([@halvarflake](https://twitter.com/halvarflake)) started work in reverse
engineering and digital rights management in the mid-90s, and began to apply
reverse engineering to vulnerability research shortly thereafter. He pioneered
early windows heap exploitaiton, patch diffing / bindiffing and various other
reverse engineering techniques. In 2004, he started zynamics, a company focused
on reverse engineering technologies. He continued to publish about reverse
engineering, ROP gadget search, and knowledge management technologies in
relation to reverse engineering. In 2011, zynamics was acquired by Google, and
Halvar spent the next few years working on defensive technologies that leveraged
the then hot buzzwords “big data” and “machine learning”. In summer 2015, Halvar
received the lifetime achievement Pwnie, and decided to take a year off to
travel, read, and surf. Since November 2016, he is back at Google.

[Slides](/archives/2017/Thomas_Dullien-Keynote.pdf)

### Nail in the JKS coffin [Slides](/archives/2017/BSidesZH_tobias_ospelt_nail_in_the_jks_coffin.pdf)

Tobias Ospelt (@floyd_ch, https://github.com/floyd-fuh/)

The Java Key Store (JKS) is the Java way of storing one or several cryptographic
private and public keys for asymmetric cryptography in a file. While there are
various key store formats, Java and Android still default to the JKS file
format. JKS is one of the file formats for Java key stores, but JKS is
confusingly used as the acronym for the general Java key store API as well. This
presentation explains the security mechanisms of the JKS file format and how the
password protection of the private key can be cracked. Due the unusual design of
JKS the developed implementation can ignore the key store password and crack the
private key password directly. Because it ignores the key store password, this
implementation can attack every JKS configuration, which is not the case with
most other tools. By exploiting a weakness of the Password Based Encryption
scheme for the private key in JKS, passwords can be cracked very efficiently.
Until now, no public tool was available exploiting this weakness. This technique
was implemented in hashcat to amplify the efficiency of the algorithm with
higher cracking speeds on GPUs.

### How I met your browser: going incognito doesn’t hide your browsing from Ragamuffin [Slides](/archives/2017/BSides-Zurich-How_I_Met_Your_Browser.pdf)

Alessandro De Vito (@\_cube0x8, https://github.com/MalfurionStormrage/)

Nowadays, the browser represents the gate between a human and its virtual world;
all this makes it one of the most challenging attack vectors and a source of
invaluable relevance during a forensic analysis. In this talk I will introduce
theoretical and practical methodologies to perform an analysis of the Google
Chrome web browser address space, dissecting – in a forensically-sound manner –
the data structures implemented by the Blink rendering engine and its JavaScript
V8 engine. In addition, some case studies will be presented with the help of
Chrome Ragamuffin, a new Volatility plugin that makes the analyst able to gain a
new set of artifacts otherwise unattainable by existing forensic tools. This
way, it also overcomes in fact the limits introduced the modern anti-forensic
techniques such as the incognito mode.

### Setting up persistent backdoors like a Russian spy

Gianni Gnesa (@GianniGnesa)

The past few years have witnessed a great number of data breaches, leaks and
hacks. Most of whom have gone undetected for weeks, months, and in some cases
even years. Considering the fact that many of the companies hit use
state-of-the-art security products (e.g. Firewall, AV, IDS/IPS, SIEM, etc.), one
cannot help but wonder: how can malicious hackers stay undetected for so long
and what kind of software do they use to keep a foothold in their victims’
networks? In this talk, we will try to answer both these questions by taking a
look at two examples of persistent backdoors. One commonly used by penetration
testers, the Meterpreter’s persistence.rb script, and another one discovered by
Mandiant while analyzing the malicious tools of the Russian hacker group
referred to as APT29.

### The Social Networks of the Security Community [Slides](/archives/2017/BSidesZH-Jeroen-TheSocialNetworksOfTheSecurityCommunity.pdf)

Jeroen Massar (@jrmassar, https://github.com/massar)

The word Networking has two meanings in the ears of today’s computer engineer:
the Internet and “social network”. Both are dear to the heart of many in the
audience, but often maintaining both up to an adequate level is a tricky affair
as one already get too much fake news, updates and other information to read on
a daily basis. Receiving the right amount of information is a very important
thing as getting too much information can cause either information overload
(reload this page and check again 😉 and on the flip side it can cause filter
bubbles if the breadth of information is too focused causing one to miss
something that might actually have been important. One important aspect of a
good social network is that having proper connections in the social networks
means that it will enable one to more easily reach out to others for help in the
community when one needs detailed information or a direct contact to resolve an
immediate answer. The talk will discuss how various communities around the world
enable such efficient communication and how one can become a part of these and
how one should be participating in them. It will also cover how one can
proactively setup communications to make sure that people who are not in one’s
bubble know how to reach you too and which drink is preferred to be drunk at the
events being organised.

### Breaking security controls using subdomain hijacking [Slides](/static/archives/2017/bsideszh-Daniel.pdf)

Daniel Stirnimann (@seckle_ch, https://github.com/stirnim)

Todays Internet heavily makes use of DNS. Not only to communicate with a target
host but also for retrieving additional information for a domain name. In fact,
many security controls relay on DNS. Anti mail spoofing is one example which
makes use of DNS zone records (e.g. SPF, DKIM, DMARC). Another example is domain
validated TLS certi cates. One would think that given the importance of DNS that
domain holders or administrators validate or monitor their zone content
constantly. Unfortunately, this is far from the truth. The reality looks more
like nobody cares about DNS, it’s biggest problem is that it finds a way to work
even if it is heavily broken (e.g. misconfigured, forgotten hostnames,
glue-record mismatch, etc.). This presentation will show real world examples of
subdomain hijacking with the consequence of breaking security controls used by
the domain names. We show how to break DMARC policies or issue TLS certificates
or simply hijack a subdomain for high profile domain names. We discuss how we
can use open data on the Internet to get a glimpse on DNS records for any domain
name. We also present a tool to validate your own zone which can be used by
administrators to detect abandoned hostnames.

### Triple Play – Triple Fail [Slides](/static/archives/2017/3xplay_3xfail_public.pdf)

Antoine Neuenschwander (@ant0inet)

By the end of this year, Swisscom plans to shut down the venerable Public
Switched Telephone Network (PSTN) in Switzerland. In a considerable endeavour of
technical operations and marketing campaigns, telcos are currently migrating
bulks of analog telephone and ISDN subscribers to so-called ‘All IP’. Voice
telephony, HDTV and broadband Internet; from now on this trinity of services
shall be provided solely over the Internet Protocol, decoupling the services
from their corresponding access medium, be it copper, cable or fibre. The plain
old telephone service is now over a hundred years old, and cable TV is also
rather antiquated; taking this step is economically and technologically
worthwhile. However, as obsolete as they are today, these technologies have
evolved to become as reliable and secure as can be. Do you remember Phreakers
and Pay-TV crackers? Introducing new ‘All IP’ services naturally bears certain
risks, as for all new technologies they have yet to mature. Last fall I upgraded
my link from a landline with DSL to FTTH and at the same time I also switched to
‘All IP’. My ISP provides the terminal equipment to the customers. It features
several ports to connect phones, computers and TV, and the fibre WAN port. I was
curious about the device’s operation, so I invested some time to look at the
communication on the WAN port, and I did find a phreakin’ vulnerability…
