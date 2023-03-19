---
title: "Talks and abstracts"
date: 2019-09-14
draft: false
featured_image: "/images/bsides_logo_blue.jpg"
featured_image_desc: "BSides Zurich logo"
---

## Keynote

{{< figure src="/archives/2019/keynote.jpg" height="300px" class="img-center mt0 fl" >}}

Nex (Claudio Guarnieri, [@botherder](https://twitter.com/botherder)) is a
security researcher and a free software developer. He researches the use of
technology as a mean for repression, and provides assistance to human rights
organizations, journalists, and activists with issues of computer security,
privacy and surveillance. He works as a Senior Technologist and Researcher at
[Amnesty International](http://www.amnesty.org/), he is an Adviser to the
[Citizen Lab](https://citizenlab.org/), University of Toronto, and a core member
of [The Honeynet Project](http://www.honeynet.org/). Nex also co-founded
[Security Without Borders](https://www.securitywithoutborders.org/). He created
the open source malware analysis software
[Cuckoo Sandbox](http://cuckoosandbox.org/), [Viper](http://viper.li/) and runs
the [Malwr](https://malwr.com/) free service.\*\*

In recent years Nex devoted his attention especially to issues of privacy and
surveillance and he published numerous articles on surveillance vendors such as
_FinFisher_ and _HackingTeam_ with the
[Citizen Lab](https://citizenlab.org/category/author/claudio-guarnieri/) as well
as on NSA/GCHQ and Five Eyes surveillance capabilities with _The Intercept_ and
_Der Spiegel_. Nex is also an opinion writer and columnist and some of his work
has been published by _Die Zeit, Slate, Deutsche Welle_ and _Motherboard_. He
has also spoken to numerous conferences including _BlackHat, Chaos Communication
Congress, Re:publica_ and many more.

He has been selected among the
[50 persons of the year 2014](http://www.wired.it/attualita/tech/2014/12/29/50-persone-wired-2014/)
by _Wired Italy_, he collected with the _Citizen Lab_ the
[EFF Pioneer Award](https://www.eff.org/awards/pioneer/2015) 2015, and he’s been
selected by _Forbes_ among the
[30 Under 30](http://www.forbes.com/30-under-30-2016/enterprise-tech/) honorees
for 2016.\*\*

Nex is also an artist, working with traditional media as well as with new and
generative media art. Most of his work deals with privacy, surveillance, and the
digitisation of modern society. Some of it has been exhibited and published in
print in Berlin and London.

### Behind the scenes of 5G security

- [Slides](/archives/2019/BSidesZH19-R_Borgaonkar-5G_Security.pdf)

_Ravishankar Borgaonkar ([@raviborgaonkar](https://twitter.com/raviborgaonkar))_

There are so much discussions around 5G security than its benefits to our
digital society. Though 5G security architecture has been evolved from 4G, it
does introduce a new service-based architecture to the existing complex and
multi-layer cellular networks.This talk will provide some ground truth on 5G
security evolution and outline potential risks in the post-deployment era. In
addition, we reveal vulnerabilities in different parts of the 5G network.

### Binary Code Similarity Search – State of the Art and Applications

_Jonas Wagner ([@\_jwagner](https://twitter.com/_jwagner))_

Finding binary code similarities has always been a valuable tool for
vulnerability detection, actor attribution and reverse engineering. One
successful approach is comparing control flow graphs of code functions based on
hand-crafted features (BinDiff, Diaphora, etc.) to identify similarity. This
approach has major drawbacks due to its high computational complexity, which
makes it inherently hard to scale and the reliance on expert knowledge about
well suited features for binary code similarity. Recently, new approaches from
academic and non-academic sources have emerged, which started using machine
learning techniques to embed code functions as similarity preserving
representations with low dimensionality. These representations are learned based
on large corpuses of data and try to reduce the reliance of expert knowledge as
much as possible. Furthermore, the low dimensionality of these representations
allow for efficient similarity searches, even when considering millions of code
functions. We will present one of these approaches and go into the details of
its functionalities, as well as experiments showing the quality of search
results over large binary corpuses. As good as these new approaches are, finding
binary code similarities at scale is still a hard problem and many intricacies
lead to some irrelevant or incorrect results.

### Microarchitectural Attacks – hype or serious threat?

_Michael Kurth ([@mik\_\_](https://twitter.com/mik__))_

Since the discovery of Spectre and Meltdown at the beginning of 2018,
microarchitectural attacks have gained increased attention outside of InfoSec
academia and industry. With the release of the MDS attacks in May this year,
speculative execution attacks moved away from using the CPU cache as shared
medium between the attacking and victim process further down the pipeline to
CPU-internal buffers. You might ask yourself, where are these vulnerabilities
coming from, how do they work, what can an attacker achieve with them and how
does it impact my threat model? In my opinion it is important for InfoSec people
to understand what goes beyond “normal” software vulnerabilities, how to
classify them and how they affect our threat models. There is a lot of hype and
fear mongering in the media around these kind of CPU vulnerabilities. This talk
will provide you with the background facts, the understanding and give you the
right mindset in order to make your own educated decisions for the
infrastructure you are responsible for. During the talk we will touch on
speculative execution vulnerabilities like Spectre and Meltdown as well as the
latest MDS attacks. We will discuss how such attacks can be used to read out
local passwords or compromise shared cloud infrastructure. All these attacks
require some knowledge on how CPUs and memory accesses work which will be
presented in a short computer architecture primer.

### Nos Oignons – Operating large Tor relays in France

- [Slides](/archives/2019/BSidesZH19-J_Voisin-TOR_Nos_Oignons.pdf)

_Julien Voisin_

Nos Oignons is a French association (https://nos-oignons.net) created in 2013
with the goal of running large Tor (https://torproject.org) exit nodes. Running
this kind of service can be challenging, both from a technical than from a
social point of view: interactions with Law Enforcement Officers, dealing with
attacks and spams, fighting the negative image of the Tor network, etc. But in
2019, we’re still alive and doing great, so we think that it could be
interesting to share our experience, and maybe inspire other people to come
together, and create similar entities, by building on top of what we’ve learned
in 6 years of existence, controlling around 2% of the exit capacity of the Tor
network!

### Swiss Cybervoting PIT(falls)

- [Slides](/static/archives/2019/BSidesZH19-J_Kirschner-Swiss_Cybervoting_PIT_falls.pdf)

_Jannis Kirschner ([@xorkiwi](https://twitter.com/xorkiwi))_

The Swiss democracy is one of it’s kind. Digitalization affects even our most
critical processes, such as voting. When a piece of code suddenly gets
responsible for democracy, it’s only natural that the voices get loud and it
raises many questions. Is our democracy at stake? Do we have to fear for our
privacy? Is electronic voting even feasible in Switzerland? Is such a solution
secure? As part of a mandatory Public Intrusion Test (PIT), the Swisspost
released their source code to the world and started a heated debate – far beyond
the Swiss borders. Not only the codebase revealed several problems during the
PIT. Interesting scoping, redefining the term “open source” and unreleased
security audits were only some of the issues that caused controversy. We will
have a look at many technical and non-technical aspects of the e-voting solution
and PIT. This talk provides an exclusive “behind the scenes” view from the
perspective of a security researcher. It invites researchers and C-level alike
to have an interesting discussion about voting security, bug bounty programs and
critical infrastructure.

### Why Johnny can’t scan at hyperscale – Tales and adventures building security scanning at Google

- [Slides](/static/archives/2019/BSidesZH19-SLekies_CCriscione-Why_johnny_cant_scan_at_hyperscale.pdf)

_Claudio Criscione ([@paradoxengine](https://twitter.com/paradoxengine)),
Sebastian Lekies ([@slekies](https://twitter.com/slekies))_

How do you lock an entire building worth of engineers out in the cold? How do
you wreck hard-science experiments worth thousands of dollars? How do you bring
down the most widely used application in the world (ok, not quite down – let’s
say how do you give a hard time to its Service Reliability Engineers)? Is it
some sort of ultra-advanced ROP-based CyberAPT? We’ve got bad news and good news
for you. The bad news is that all it takes to do these things might be a
security scan. The good news is that it can also do good things for you, like
preventing that VM from being owned 5 minutes after going online. This talk
presents a few years worth of experiences scanning the hyperscale environment at
Google, with an overview of the landscape of security scanning technologies and
plenty of war stories. We have built security scanners covering all layers of
the stack, integrated them with vendor-built systems, operated them for many
quarters and watched them fail in all sorts of interesting ways. The security
scanning world, in particular at scale, is largely dominated by hand-wavy white
papers and by internet-wide security scan research focusing on a small subset of
the problem space. Having to identify vulnerabilities on millions of devices and
countless web applications and actually get them fixed, presents its own set of
technological and process-related challenges beside maximizing network
throughput on a single machine. Traditional one-size-fits-all approaches to
security scanning with regular scheduled network scans or even the more modern
Agent-based variants, don’t always work at hyperscale. The audience will walk
away with the understanding of a whole new set of challenges for the field:
real-world-compatible continuous scanning, faster-than-humans preemptive
automation, logical inventorying and targeting, and transparent scanner
engineering. While they are exacerbated by scale and particularly nasty at
hyperscale, they are just as real in smaller environments.
