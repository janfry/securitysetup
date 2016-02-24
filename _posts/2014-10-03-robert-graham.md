---
layout: post
title: Robert Graham
redirect_from: "/home/2014/10/3/robert-graham/"
category: Guests
---

**Who are you, and what do you do?**

My name is [Robert Graham][1]. I write lots of code. I hack lots of things. I write lots of [blogs][2].

**What hardware do you use?**

My desktop is an old 6-core Nehalem system with 24-gigs of RAM with a Radeon 6790. These are fairly old specs, but really, modern specs aren't significantly faster than this. My laptop is a MacBook Air 2012, 13-inch. I split my time about half-and-half between them.

I have a three monitor setup, a 30-inch 2560x1600, a 19-inch 1280x1024 to the side, and a 42-inch 1080p TV up above. The TV is for BluRay or NetFlix, it's too impractical to do anything useful on. I restrict myself to the two monitors because I keep losing the damn mouse pointer when there's too many.

The coolest thing about my setup is that the computer is in the closet on the other side of the wall. USB and monitor cables go through a hole in the wall to the other side. It means the room is utterly quiet without fan noise. Even with password cracking going with the fan set manually to high, I still can't hear the loud computer on the other side of the wall.

My desktop boots from an SSD, with a mirrored 3-terabyte drives for local storage. For mass storage, I have a Synology 8-bay NAS with 3-terabyte drives in a RAID6 configuration (18-terrabytes). It's dual 1-gig Ethernet from the desktop to the hub to the NAS. The hub is a 24-port managed hub (for doing things like setting up monitor ports to watch things). I had to upgrade the hub to get link aggregation to work.

In addition, the desktop has a quad-port RAID card with four SSD drives that delivers 1.6 gigabytes-per-second of bandwidth on reads. Among the things I do is write very fast file and network parsers, which are much faster than network drives. Therefore, I need a fast enough drive so that it's not the bottleneck. So, for example, my DNS server that I wrote parses the 8-gigabyte .com zonefile about 3 times faster than 'wc' (wordcount), or about 30 seconds. Being that 'wc' is a damn simple parser, and the DNS server must not only parse but also insert the records into the database, this is really fast. The upshot is that if I don't have a quad SSD RAID, the disk rather than my code becomes the bottleneck. Also, Diablo III loads insta-fast off the quad SSDs :)

The desktop and the laptop are old because my hardware budget goes to other things. I have a mini-rack with an 8-port 10-gbps Ethernet hub, with three servers attached: quad-core 3-ghz IvyBridge  server processors with 32-gigs of RAM and a dual port 10-gbps Ethernet card. These servers are 1U half-length tiny devices: there's just enough room for the motherboard, the Ethernet card, and an SSD boot drive. This little rack allows me to do 10-gbps testing with things like my [masscan ][3]port scanner or my DNS server.

Also, I have a five Radeon 290x system mining Litecoin, which I occasionally also use for password cracking. The lesson here is that having the latest graphics cards in your desktop is for chumps – they should be in your cracking/mining server.

I also have a variety of build machines like Raspberry Pi and "netbooks" that automatically download my software every night and build/regression test it. I have a little MacMini with a lot of RAM as the test target, running a bunch of different target servers in VMs.

I have only 75-mbps connection to the Internet, which is sufficient to shelling out to hosting environments where I have 1-gbps connections for doing things like Internet scanning.

**And what software?**

My desktop runs Windows, though always with a Linux VM in the background (usually [Kali][4], though sometimes Ubuntu, or both). Partly this is because Linux desktops are still a pain, it's just a ton easier running Windows with Linux in a VM. Partly this is because Microsoft's [VisualStudio ][5]programming environment is much better than anything on Linux. I'm not trolling here. My standard paradigm is to write a few lines of code, then step through with the debugger to make sure what I wrote works, then write a few more lines of code. This works in VisualStudio, this doesn't work well in any Linux environment I've tried, though Eclipse will work in a pinch.

My laptop runs Mac OS X most of the time, mostly to use XCode to debug Unixy things that don't work on Windows. XCode is not as friendly to debugging as VisualStudio, but it's still a lot better than Linux stuff. I also have Bootcamp loaded with Windows, but I find I use Windows less and less on the notebook. More and more, apps are just inside Chrome, so operating system doesn't really matter.

Other than that, I use the standard apps: Chrome, Word, PowerPoint, Google Docs.

**What would be your dream setup?**

What I have, except I'd like a 10-gbps connection to the Internet for insane scanning.

**How do you streamline your workflow?**

Two years ago I got an 18-terabyte NAS. It means I stop having to manage disk space, and helped me organize all the data tremendously. I use the cloud, like [github][6], to organize things as well. These days, if I have file, I always know where it is. In the past, I had to hunt across slow disks to find it.

[1]: https://twitter.com/erratarob
[2]: http://blog.erratasec.com/
[3]: https://github.com/robertdavidgraham/masscan
[4]: http://www.kali.org/
[5]: http://msdn.microsoft.com/en-US/vstudio
[6]: https://github.com/
