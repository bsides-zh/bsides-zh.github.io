---
title: "Talks and abstracts"
date: 2018-09-22
draft: false
featured_image: "/images/bsides_logo_blue.jpg"
featured_image_desc: "BSides Zurich logo"
---

## Keynote

{{< figure src="/archives/2018/keynote.jpg" height="300px" class="img-center mt0 fl" >}}

Vincenzo Iozzo ([@\_snagg](https://twitter.com/_snagg)) Vincenzo is a Senior
Director at CrowdStrike Inc. Prior to this, he was the CEO and Co-Founder of
IperLane, Inc. In addition, Vincenzo is an Associate Researcher at the MIT Media
Lab. Vincenzo is a Network Leader for Village Global, a seed stage VC fund based
in Silicon Valley. He serves as a committee member on the Black Hat Conference
board and is a co-author of the “iOS Hacker’s Handbook” (Wiley, 2012). Vincenzo
also co-authored the winning attacks against Firefox, iOS and BlackberryOS at
Pwn2Own from 2010 to 2012.

[Slides](/archives/2018/BSZH18-Keynote-Iozzo-Future_offense_public.pdf)

### Angad: A Malware Detection Framework using Multi-Dimensional Visualization [Slides](/archives/2018/BSZH18-AnkurTyagi-angad.pdf)

_Ankur Tyagi ([@7h3rAm](https://twitter.com/7h3rAm), <https://github.com/7h3rAm>)_

Angad is a framework to automate classification of an unlabelled malware dataset
using multi-dimensional modelling. The input dataset is analyzed to collect
various attributes which are then arranged in a number of feature vectors. These
vectors are then individually visualized, indexed and then queried for each new
input file. Matching vectors are labelled as per their AV detection categories
for now but this could be changed to a heuristics approach if needed. If dynamic
behavior or network traffic details are available, vectors are also converted
into activity graphs that depict evolution of activity with a predefined time
scale. This results into an animation of malware/malware category’s behavior
traits and is also useful in identifying activity overlaps across the input
dataset.

### Building a End-to-End Open Source Container Security Stack

_Henri Dubois-Ferriere ([@henridf](https://twitter.com/henridf),
<https://github.com/henridf>)_

Cloud Native platforms such as Kubernetes help developers to easily get started
deploying and running their applications at scale. But as developers push out
updates at a faster rate, and as the barrier between dev, ops, and sec gets
blurrier, how you secure and maintain compliance standards in these environments
becomes extremely important. To answer this question we’ll describe an
end-to-end security stack, built only with open source components. We will cover
the entire process, starting with approaches to do image scanning inside your
continuous integration process. Then we’ll talk about runtime security and
finally forensics, with a focus on volatile containers that are frequently
started, migrated, and updated in an orchestrated environment like Kubernetes.
Here we’ll dig into tools like Anchore, CoreOS Clair, and Sysdig Falco.
Attendees will walk away with a good understanding of the challenges of securing
a Cloud Native platform and practical advice on using open source tools as part
of their security strategy.

### Data Breaches: Barbarians in the Throne Room [Slides](/archives/2018/BSZH18-Dave_Lewis-ThroneRoom.pdf)

_Dave Lewis ([@gattaca](https://twitter.com/gattaca))_

Often defenders worry about the intangible security problems. Defenders need to
concentrate their efforts defending the enterprise by focusing on the
fundamentals. Too often issues such as patching or system configuration failures
lead to system compromise. These along with issues such as SQL injection are
preventable problems. Defenders can best protect their digital assets by first
understanding the sheer magnitude that a data breach can have on an enterprise.
In this talk I review my findings after analyzing hundreds of data breach
disclosures as it pertains to what went wrong. I had previously done this for
2016 and I will have the 2017 review ready by the time of this talk.

### IoT PenetrationTesting – A Deep Dive into Hidden Flaws

_Saurabh Swaroop_

The presentation is aimed at disclosing the various hard to find vulnerabilities
in IoT ecosystem. While we have billions of IoT device in cyberspace most still
lack in basic security. One of the most important and hard to test part of IoT
device is its firmware and vulnerabilities at hardware level. This talk will be
aimed at understanding IoT ecosystem, identifying attack surfaces, reverse
engineering the firmware, understanding firmware file systems, extracting
standard and non standard sections from firmware, performing static, dynamic and
behavioural analysis of firmware as well as hardware hacking. Talk will be
accompanied with demo showing digging the firmware for various secrets,
emulating cross platform binaries, fuzzing and finding buffer overflows,
hardware hacking (SPI,UART,I2C). Talk and demo will be done with open source
tools so audience can gain maximum from it. The major takeaways of the talk will
be deep insight and understanding of pen testing IoT devices.

### The Politics of Public Attribution

_Florian Egloff ([@egflo](https://twitter.com/egflo))_

Doxing each other, dropping private information on the internet for the public
to see, has cultural roots in the hacking community. However, cybersecurity
researchers were surprised when intelligence agencies, who traditionally prized
their secrecy, followed suit and revealed details on other countries’ cyber
operations. An increasing number of states have published information regarding
cyber espionage operations discovered on networks within their jurisdiction. So
far, little research has been published analyzing what motivates such behavior.
Understanding why states chose to publish sensitive details is important, as
practices of strategic interaction in cybersecurity are only just emerging into
public view. This talk will offer a rough account of the identified practices in
selected empirical cases and offer first possible explanations on what the
respective strategic communities may have wanted to achieve when releasing such
information. The talk is based on a larger empirical research project looking
into this question. Particularly, I will argue that more states investing in
attribution capabilities (both on the intelligence and policy side) has changed
the strategic context, the result of which we are now seeing. Drawing on
research from political science, the talk contributes towards bridging the gap
between policy and information security communities. The talk is aimed at
information security professionals, who would like to better understand the
politicization of their field. Focusing on a controversial topic, public
attribution, this talk will contribute towards a more comprehensive
understanding of what public attribution is used for at the state level.

### SCION – an Internet Architecture to survive the 21st Century

_Raphael M. Reischuk ([@raphaelreischuk](https://twitter.com/raphaelreischuk))_

The Internet has been successful beyond even the most optimistic expectations.
It permeates and intertwines with almost all aspects of our society and economy.
The success of the Internet has created a dependency on communication as many of
the processes underpinning the foundations of modern society would grind to a
halt should communication become unavailable. However, much to our dismay, the
current state of safety and availability of the Internet is far from
commensurate given its importance. Although we cannot conclusively determine
what the impact of a 1-day, or 1-week outage of Internet connectivity on our
society would be, anecdotal evidence indicates that even short outages have a
profound negative impact on society, businesses, and government. Unfortunately,
the Internet has not been designed for high availability in the face of
malicious actions by adversaries. Recent patches to improve Internet security
and availability have been constrained by the current Internet architecture,
business models, and legal aspects. Moreover, there are fundamental design
decisions of the current Internet that inherently complicate secure operation.
Given the diverse nature of constituents in today’s Internet, another important
challenge is how to scale authentication of entities (e.g., AS ownership for
routing, name servers for DNS, or domains for TLS) to a global environment.
Currently prevalent PKI models (monopoly and oligopoly) do not scale globally
because mutually distrusting entities cannot agree on a single trust root, and
because everyday users cannot evaluate the trustworthiness of each of the many
root CAs in their browsers. To address these issues, we propose SCION, a
next-generation Internet architecture that is secure, available, and offers
privacy by design; that provides incentives for a transition to the new
architecture; and that considers economic and policy issues at the design stage.
Within roughly 100 person years, we have implemented SCION and deployed it
(among others) in the production networks of two Swiss ISPs.
