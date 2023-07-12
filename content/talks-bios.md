---
title: "Talks & Bios"
date: 2023-05-10
draft: false
menu:
  main:
    weight: 4
---

## Keynote

{{< figure src="/images/keynote.jpg" height="300px" class="img-center mt0 fl" >}}

**Myriam Dunn Cavelty** is a Senior Lecturer for Security Studies and Deputy for
Research and Teaching at the Center for Security Studies (CSS) at ETH
Zurich. She studied International Relations, History, and International Law at
the University of Zurich. She was a visiting fellow at the Watson Institute for
International Studies (Brown University) in 2007 and fellow at the stiftung neue
verantwortung in Berlin, Germany 2010–2011.

Her research focuses on the politics of risk and uncertainty in security
politics and changing conceptions of (inter-​)national security due to cyber
issues (cyber-​security, cyber-​war, critical infrastructure protection) in
specific. In addition to her teaching, research and publishing activities, she
advises governments, international institutions and companies in the areas of
cyber security, cyber warfare, critical infrastructure protection, risk analysis
and strategic foresight.

You can find more information on her work and publications on the
[official ETH website](https://css.ethz.ch/en/center/people/dunn-cavelty-myriam.html)

## Talks

### Tracking threat actors based on publicly available data

Most malware campaigns are carried out in different phases. If we focus on
attacks that affect the endpoint, web downloads and e-mails are the preferred
initial access vectors. In both cases, a so-called dropper or loader is usually
distributed as the first stage. If an infection occurs, the second stage, based
on the initial choice, is either unpacked or downloaded from a payload delivery
server. If this payload is executed, it connects to a command-and-control
server, where the attacker gives specific instructions and thus controls the
post-infection phase. During these phases, the malware repeatedly contacts
attacker-controlled infrastructure. In this talk we want to focus on these
infrastructures and try to identify and report them as quickly as possible using
publicly available information.

**Bio:** Patrick Schläpfer - [@stoerchl](https://twitter.com/stoerchl)

Patrick is a malware analyst. Whether he is manually reversing malware or
tracking threat actor infrastructures based on their domains, in almost any
security area he has interest and curiosity guiding him.

### Golden mistake

In my presentation, I will focus on the anomalies that can occur when
adversaries utilize golden tickets and the methods to detect these anomalies.
The primary point is not the process of stealing the krbtgt account hash. I
believe the artifacts surrounding the use of golden tickets are more relevant
than how the theft of a krbtgt hash occurs. Using > stealing The use of golden
tickets generates a lot of artifacts and anomalies that should be monitored and
detected.

**Bio:** Alexander Rodchenko

Alexander Rodchenko is senior SOC Analyst at SOC Security Research Group for
Kaspersky, with responsibility for investigating industry events and trends,
monitoring and threat hunting. Joining Kaspersky in 2016 as an analyst in SOC
Security Research Group, Alexander was engaged in the international forum of
practical cybersecurity PHDays in 2019 and 2021, where – as an experienced
speaker - he presented his discoveries on SOC as a way of detecting abnormal CLR
activity. Beginning his career with OJSC RosNeft, he led industrial safety,
troubleshooting and audits. Alexander now uses his expertise to advise customer
threat detection/hunting teams on the appropriate responses for threats and
trends.

### Paralyzing the Node one RegEx at a time

Imagine a single input being able to takedown millions of websites. This talk
delves into the significant yet frequently underestimated world of Regular
Expression Denial of Service (ReDoS) vulnerabilities and their significant
threat to modern web applications. We first provide a primer on the often
overlooked vulnerability class and explain how it affects different popular
runtimes. After, we share our research findings from scanning the most popular
packages en-mass, revealing the existence of unsafe expressions in critical
libraries that underpin millions of applications.

**Bio:** Elliot Ward

Elliot is a security researcher @ Snyk, with many years working on application
security and offensive security topics. Elliot is from the United Kingdom but
has been living in Zurich now for 6 years. He enjoys hacking, craft beer, cats,
skateboarding and snowboarding.

### TA505 and the Dark Side of GoogleAds: Unraveling the Dangerous Campaigns

The e-crime group TA505 has been observed to leverage campaigns using Google
Ads. The Command and Control (C&C) server used in this latest campaign was
reportedly recycled from a similar operation that took place on February
7th 2020. The similarities in the initial attack chain, including the reuse of
the C&C server, is in line with the group’s operations. The group's modus
operandi usually involves a multi-stage process of downloaders and short-lived
C&C servers. The recent campaigns and the use of new tools shed light on the
group's evolving tactics, which now seem to target not just organizations by
extortion and file encryption using the infamous Cl0p ransomware, but also
regular individuals' cryptocurrency wallets and accounts.

**Bio:** Antonis Terefos - [@Tera0017](https://twitter.com/Tera0017)

Antonis Terefos is a Threat Intelligence Researcher focusing on Cybercrime. His
expertise includes reverse engineering, malware analysis and creating tools
automating malware reversing.

### How to break, then fix, differential privacy on finite computers

Differential privacy is a provable approach to publishing or releasing insights
from sensitive data, without inadvertently leaking individual information. In
many ways, differential privacy is like cryptography: even though its basic
building blocks are conceptually simple, their implementation can be
surprisingly tricky. This talk presents the result of our applied research about
floating-point vulnerabilities on differential privacy implementations. First,
we explain what it means for differential privacy software to be vulnerable to
attacks, and how to reason about the severity of such vulnerabilities. Second,
we present precision-based attacks, a new class of vulnerabilities which affects
several open-source libraries. Finally, we outline a new technique to address
this vulnerability, and all other possible attack vectors based on
floating-point behavior.

**Bio:** Damien Desfontaines - [@TedOnPrivacy](https://twitter.com/TedOnPrivacy)
(Twitter), [@tedted@hachyderm.io](https://hachyderm.io/@tedted) (Mastodon)

Damien works as a Scientist at Tumult Labs, a startup focusing on making it
easier to share or publish insights from sensitive data, using differential
privacy. Before that, he led the anonymization consulting team at Google, and
got his PhD in Computer Science from ETH Zurich.

### Cultural Differences in Social Engineering: A Swiss Perspective

This talk will discuss the role of cultural differences in social engineering
attacks in Switzerland. Examples of real-world attacks will be presented based
on what cultural differences made them successful.

**Bio:** Dominik Nufer -
[LinkedIn](https://www.linkedin.com/in/dominik-nufer-7720a0a6/)

As a senior security tester, Dominik improves the integral security of a wide
range of systems and organizations: from electronics and networks to web
applications, attack simulations and social engineering. After working as a
software engineer for over ten years, he joined the testing team at Redguard AG
in 2016. Dominik not only tests systems and hardware, but also additionally
leads one of the technical security testing teams at Redguard AG. He holds a
Master of Advanced Studies in Information Technology with specialization in
Security (BFH Bern) and teaches at BFH in the area of Internet of Things (IoT).
