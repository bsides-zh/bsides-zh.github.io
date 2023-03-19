---
title: "Talks and abstracts"
date: 2022-09-17
draft: false
featured_image: "/images/bsides_logo_blue.jpg"
featured_image_desc: "BSides Zurich logo"
---

## Keynote

{{< figure src="/archives/2022/keynote.jpg" height="300px" class="img-center mt0 fl" >}}

**Sanaz Yashar** is a senior manager at Mandiant. In this role, she assists EMEA
government agencies and commercial organizations in uncovering today’s most
advanced threats, while also providing feedback on the various threats
specifically targeting the Middle East.

Her holistic analysis provides organizations a strategic level of insight into
the potential operational impact of advanced threats, while also providing
hands-on hunting and remediation recommendations.

Prior to joining Mandiant, Sanaz was director of threat intelligence at an
Israeli cybersecurity company. She has over 15 years’ experience with the Israel
Defense Forces, working within the elite intelligence unit, specializing in
variety of novel cyber operations.

Her experience as an Intelligence officer, combined with her Middle Eastern
background, allows Sanaz to provide a unique kind of threat analysis from the
attacker’s point of view and mindset to give a focused, proactive solutions.

Sanaz was born in Tehran, Iran and immigrated to Israel, where she earned her
Bachelor of Science degree from Tel Aviv University and MBA degree from Ben
Gurion University.

### Surviving “Agile” as a security team (and become friends with the DevOps crowd)

DevOps and agile processes have proven efficient and are here to stay. Security
teams are mostly still very skeptical as they have to act as gatekeepers and
don’t have enough resources to keep up with the increased speed of changes. This
causes friction between DevOps and security teams. This talk will dig deeper
into the mindset of DevOps teams, how they function, what the security teams can
do to support them (and the other way around) and what needs to change in order
for the security teams to not stand in the way of DevOps, but rather be a part
of it and get true DevSecOps going.

**Bio:** Sven Vetsch – [@disenchant](https://twitter.com/disenchant)

Co-Founder and Head of Security Research at Redguard. Mainly into application
security for the last 15+ years. Currently focusing on “agile security”,
DevSecOps as well as container and Kubernetes security.

### Windows Hardening – How hard can it be?

The default settings of Windows are not secure. Security as well as privacy
settings have to be defined and implemented by users and administrators or
companies themselves. Microsoft offers different ways to configure a (secure)
system, traditionally via group policies, in the cloud age with Intune. There
are thousands of settings with multiple choices. It takes an awful lot of time
and effort to find out which of these settings are necessary and what the impact
of them is. So that not everyone has to reinvent the wheel, there are various
guidelines such as Microsoft Security Baseline, CIS Benchmark or BSI SiSyPHuS.
In the talk, we will discuss how these guidelines differ and how to proceed to
define one’ s own policy. We also try to shed light on how you create your own
guideline and what you need to look out for.

However, the definition of policies is only one side of the coin. We also want
to check whether the predefined configuration has been correctly and completely
applied to a system. Further we need a tool to analyse and evaluate the
configuration of a system. There are several ways to do this and there are
challenges. One option is to use standard tools such as the Policy Analyzer or
the analysis of group policy reports. HTML or XML reports must be parsed and
assessed. We talk about our experiences and pains with this procedure. For
systems that have not been configured via a central system, the group policy
report falls short and standard tools do not provide all the data for a complete
analysis. Therefore, we decided to develop our own tool. All the settings must
be gathered, interpreted and evaluated from various sources such as the
registry, audit policy or user right assignment. When evaluating settings, other
pitfalls arise, such as the language of the operating system or what the
question what score is given for the result.

**Bio:** Mirjam Blumenstein – [@cyberminza](https://twitter.com/cyberminza)

Mirjam Blumenstein works in the field of Information Security Management since
2013, first as an audit manager for a large German hosting provider, later as a
consultant for the development and implementation of ISMSs. Currently she works
as Research assistant at ZHAW, where she also earned her master’s degree in
Computer Science. During this time, she started to teach about the fundamentals
of Information security management and ISO 27001. She now spends most of her
free time with her toddler twins.

**Bio:** Michael Schneider – [@0x6d69636b](https://twitter.com/0x6d69636b)

Michael Schneider is working in information security since 2010. He works at
scip AG as a penetration tester and head of auditing. He is an expert at
penetration testing, hardening and the detection of vulnerabilities in operating
systems. He is well-known for a variety of tools written in PowerShell to find,
exploit, and mitigate weaknesses. In his free time, he is a driver of classic
cars with Team Paddy Murphy.

### Malware, Zero Days, and PLCs, Oh Boy!

While researching Automation Direct’s DirectLogic 06 Programmable Logic
Controller (PLC), an active ecosystem of industrial password “cracking” software
was discovered targeting a range of different industrial devices (PLCs,
Human-Machine Interfaces, and PLC project files) and vendors. Analysis of a
specific variant targeting DirectLogic PLCs indicated that no cracking was done,
rather the software utilized a zero day exploit to retrieve the PLC password and
present it to the operator. Even worse, the software acted as a malware dropper
for the Sality virus – an old, yet still effective botnet typically used for
distributed computing tasks such as password spraying, cracking,
denial-of-service attacks, and cryptocurrency mining. In this talk, we will go
over the analysis and reverse engineering of this malware at a high level –
static and dynamic techniques and tools used that made the analysis easier and
defeated anti-analysis techniques. We will discuss the zero day exploit that was
embedded in the malware dropper and how we crafted a significantly more severe
version based off the original. We will also talk about the history of the
Sality malware and how it’s evolved over time. Finally, we will discuss the
industrial password “cracking” ecosystem, how the threat actors advertises their
malware on the internet, features of the malware and what that implies about the
threat actors motivations, and the consequences of an infection in an industrial
environment.

**Bio:** Sam Hanson – [@secureloon](https://twitter.com/secureloon)

Sam Hanson is a Vulnerability Analyst at Dragos, inc where he has been
researching vulnerabilities and malware targeting our critical infrastructure
for the past 2.5 years. Prior to Dragos, Sam was a student at the University of
Minnesota – Twin Cities where he studied Computer Science.

### Binary code as a searchable IOC

Many types of IOCs are searchable and a range of technologies exist to do so.
Its benefits are to support rapid incident response, confirm or exclude
breaches, detection and identification of attacks, amongst others.

The types of IOCs that are searchable are usually textual data, like application
logs, network or host indicators, hashes of files, etc.

In this talk we are going to explore the question of: what if binary code is a
searchable IOC?

We will present use cases where binary code search technologies enhances
existing threat intelligence and malware analysis processes and makes entirely
new ones possible.

More concretely, we will show how code search technology can:

Increase detection and identification resilience by focusing on fine-grained
code similarities of changing malware threats Given a binary file, hunt through
millions of binaries for similar files, as you would with log lines, IPs,
hashes, etc. Track the evolution of malware families at large scale and identify
changes over time in an automated manner Provide contextual information by
uncovering relations between unknown binary files and known binaries files from
intelligence sources We will showcase these approaches with the following,
amongst others, examples of real-world threats:

Detecting recent code changes of IcedIDs GZipLoader component Hunting for
undetected BumbleBee loader variants Tracking the multi-year long evolution of
Qbot by analysing over 500k samples The contents of this talk are based on many
years of actively developing and using code search technology on real-world
malware threats.

**Bio:** Carlos Rubio

Carlos Rubio is a malware researcher at Threatray, where
he is mainly responsible for reverse engineering malware to automate the
detection process of new threats. In addition to researching new applications
for code reuse technology that can help in different areas such as threat
hunting, incident response, tracking the evolution of malware families, among
others. He previously worked on reverse-engineering malware at Blueliv, S21sec
Counter Threat Intelligence Unit and in the Panda Security Adaptive Defense
team. He has previously spoken at Botconf (2022, 2019), Virus Bulletin localhost
2020, as well as many closed-door private conferences.

**Bio:** Jonas Wagner – [@\_jwagner](https://twitter.com/_jwagner)

Jonas Wagner is the co-founder and CTO of Threatray and has built the
technological foundation of its code search engine based on years of research
and development. He holds a Masters Degree in Cybersecurity from the Bern
University of Applied Sciences. He has previously spoken at BSides Zürich
(2019), DFRWS (2017) and many private events.

### Finding Malicious artifacts in the Wild West OSS supply-chain

In this talk we will break down the approach we have produced at Snyk to
automate the continuous detection of malicious artifacts across various open
source ecosystems to overall improve the state of software with a reliance on
third party dependencies. We will dive into our methodology and analysis
pipeline which leverages a combination of static and dynamic analysis to
highlight signals indicating malicious behavior deep within scanned artifacts,
before presenting a subset of our findings revealing the most common type of
malware found, what kinds of data is being exfiltrated, and the signals used for
detection. Our results have uncovered sophisticated malware going far beyond the
expected cryptominers, revealing targeted attacks leveraging dependency
confusion, through to artifacts deploying commercial malware in developer
workstations and application containers. We will then go into some specifics
from a targeted dependency confusion attack we identified within the NPM
ecosystem showing how such attacks are actually used in the wild, before finally
presenting our follow-up work and next steps.

Participants will expect to come away from the talk with:

An overview of the current threats to Supply Chain Security with a focus on OSS
How we have developed our custom malware detection pipeline The general results
and common malware types in open source package repositories How we played Among
Us with an adversary setting up a honeypot targeted malware which resulted in a
surprising twist! What future work Snyk are performing to detect more malware
and help clean up repos! In the breakout session we host an interactive session
where dive deep into the reverse engineering process and results from the custom
malware from the previously mentioned targeted dependency confusion campaign,
followed by an open discussion regarding additional details on our ongoing
future detection efforts, areas of improvement, follow-up research and general
Q&A.

**Bio:** Elliot Ward

Elliot is a security researcher @ Snyk, with many years working on application
security and offensive security topics. Elliot is from the United Kingdom but
has been living in Zurich now for 5 years. He enjoys hacking, craft beer, cats,
skateboarding and snowboarding.

### A Tale of Securing Containerized Workloads at Scale

In this talk, we tell the story of how we secure our containerized workloads at
Datadog. We start by laying out the real-world threats to Kubernetes
environments in 2022, showcasing some recent incidents and malware in the wild,
as well as challenges in securing containers’ supply chain and ensuring their
provenance. Then, we dive into the approaches we evaluated and took to gain
visibility and ensure no dangerous workloads run in our clusters – which,
unsurprisingly, is not straightforward when your “customer” is a fast-moving
engineering team of more than a 1’000 engineers. We discuss how using the same,
consistent rule set across different stages of the deployment lifecycle helps
gaining consistency and trust from other teams. In particular, we showcase how
to treat security rules as code, including with tests and a continuous
integration (CI) pipeline, and discuss how to balance the “cost of false
positives”‚ with the “risk of false negatives” depending on the environment you
operate in.

Throughout the talk, we advocate for a pragmatic, threat-informed and risk-based
approach to securing Kubernetes clusters without the hype. For every rule we
implement, it’s critical that we, as security engineers, are able to demonstrate
the attacks it prevents or detects backed with real-world data. We also discuss
the operating model of providing security “as a platform”, acting as enablers
for engineering teams to ship secure workloads fast.

No matter whether you run one or a hundred clusters, you will walk away with
actionable insights on how – and especially why – to secure containerized
workloads in an engineering-heavy environment.

**Bio:** Tommy McCormick – [@jan0ski\_](https://twitter.com/jan0ski_)

Tommy works as a security engineer at Datadog. He’s passionate about threat
detection and securing containerized workloads, applying pragmatic,
threat-informed security controls at scale and ensuring that “shifting security
left” isn’t just a buzzword.
