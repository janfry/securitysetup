---
layout: post
title: Adrian Pastor
category: Guests
---

**Who am I? What do I do?**

My name is Adrian Pastor. Online, I use the rather silly moniker ['pagvac'](https://twitter.com/pagvac). At my age, it feels a bit childish to continue using handles, or nicknames as they have always been known in the world of IRC (which is where I started using it). I think I can't let it go simply because I’ve been using it for so long.

I have been passionate about security since witnessing the execution of an exploit (WinNuke NetBIOS OOB) for the first time circa 1997-1998 at an Internet café in my hometown. The Internet café owner would use it against IRC users who would troll his customers. I still remember being absolutely blown away that someone could remotely freeze a computer.

I'm the CEO and co-founder at [MINERVA](http://minerva-is.net). We specialize in pentesting, security audits, and training. We pride ourselves in providing a customized service with a friendly and human touch. If you want automated security scanning services we certainly aren’t the right company for you!

I’m also a Founding Member at [GNUCITIZEN](http://www.gnucitizen.org), a collective of independent security researchers. Perhaps, my best-known work at GC was the discovery of vulnerabilities that granted remote administrative access to the BT Home Hub, the UK’s most popular broadband router.

**What hardware do you use?**

I was converted to Apple in 2010, quite late compared to most security pros I know. Several of my colleagues at the time would praise how stable and headache-free Macs were. Since this is exactly what I need when consulting for clients, I decided to follow suit. I've been a Macbook Pro user ever since.  I don’t own a desktop computer. Currently I have a mid 2012 MBP with a 15-in retina screen, 16GB RAM, and 256 GB SSD. In addition to mobility, performance is everything for me, so I usually get one of the best MBP configurations available at time of purchase.  I donated my previous MBP to my better half and it still works like a charm despite its 5 years of age!

**And what Software?**

I’m slowly migrating my security tools from various Ubuntu VMs to OS X, my host OS. While I still use VMWare Fusion for Windows software that is not available on OS X, I realized I was using VMs because of the ability to restore snapshots. This is essentially a glorified backup solution, which I’ve replaced with Time Machine. I have Time Machine configured to use two backup disks. One is Time Capsule, which continuously makes backups seamlessly in the background over WiFi. The other is an external caddy, which I plug into my MBP once a month. I use both backup disks because I worry that either disk will fail and lose critical data. I think of this as a humble version of RAID, which for me is necessary since Time Capsule doesn’t support RAID. I find security tools perform significantly better when run natively.

For security testing, I mostly use Burp (including plugins such as CO2) because of its flexibility and power. I use sqlmap to confirm the existence of SQLi vulnerabilities found manually through Burp Repeater, or automatically with Burp Scanner. Is it actually possible to gain access to the DBMS or is this just a SQL error rather than SQLi? I also find sqlmap useful in assessing the impact of SQLi vulnerabilities. Do we only have SELECT permissions, or can we also UPDATE tables? How about databases we have gained access to? Are they only a select few containing public data, or can we instead access all databases on the DBMS, including those where PII or payment data are stored? sqlmap is great to answer such questions.

If the target site is based on WordPress, running WPScan is a must, as generic vulnerability scanners such as Nessus and Qualys are quite poor at identifying more obscure CMS-specific vulnerabilities.

I also use SoapUI when testing SOAP services, mostly to create template requests which I then proxy to Burp for actual testing. I also use Oxygen to perform manual security reviews of XML schemas such as XSD.

Similarly to [Jan Fry](http://thesecuritysetup.com/2014/10/11/jan-fry/), I find SWFScan incredibly fruitful, despite it having been unmaintained for years.

When something more customized is required to identify or demonstrate the presence of a vulnerability, I tend to resort to writing scripts in bash and PHP (executed on the command line, using the 'php –r' flag). I also sometimes write in python. I must say I’m pretty terrible at python but I enjoy how elegant the code is because one is ["forced"](http://www.secnetix.de/olli/Python/block_indentation.hawk) to indent code blocks.

When testing thick clients, I use the usual suspects such as Echo Mirage, DARKER’s Enabler, Sysinternals Suite, JD-GUI, jad, JavaSnoop, Wireshark, and BinScope.

Build security reviews would be way more time consuming if it weren’t for SureCheck.

While there are other security testing tools I use, I would say the aforementioned are the ones I use most.

In terms of privacy protection, NoScript for Firefox, and AdBlock and Ghostery for Safari are must-have extensions and plugins, respectively. When using public hotspots, I use a home-grown Automator application that changes OS X’s proxy settings to use SOCKS over SSH using public key authentication. I have a shortcut for this application on my dock. As soon as I click it I have my poor man’s VPN up and running without entering any passwords since I’m using a passphrase-less private key to connect to the SSH endpoint. The endpoint is just an Ubuntu Server VPS with no sensitive data stored on it, nor superfluous daemons.

**What would be my dream setup?**

To be honest, because I move fairly often, I'm really pleased with my current setup as it's so mobile. Whenever I need access to servers, I simply enrol in a new VPS subscription. That being said, creating a serious password-cracking ‘station’ has been a dream of mine for a while. I’ve always been a bit obsessed with password cracking for some reason. The main reason I have not taken on such project yet is because I perceive anything heavy and voluminous as more junk that will only make my next move more miserable.
