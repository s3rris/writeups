# @OSINTDojo challenge

Date: Aug 8th 2022

Link: https://twitter.com/OSINTDojo/status/1556630457852121089

<img width="594" alt="challenge_tweet" src="https://user-images.githubusercontent.com/111104710/184779429-09a28176-6e8a-4aed-b029-cf3ef4ef10e0.png">

### Challenge
The three questions to answer are:

* What Web Browser did the user use?:
* What Operating System and OS version did they use?
* What is notable about this OS?

## What Web Browser did the user use?
There's quite a bit of information already available from the screenshot. This looks to primarily be a browser [User-Agent](https://developer.mozilla.org/en-US/docs/Glossary/User_agent), which helps identify the browser as well as some additional information on the operating system and platform that it's running on.

Software name: **Naenara**

A quick search for `Naenara` comes back to a number of Google results for a North Korean browser. There's a decent WikiPedia article for [Naenara (Browser)](https://en.wikipedia.org/wiki/Naenara_(browser))

> Naenara is a North Korean intranet web browser software developed by the Korea Computer Center for use of the national Kwangmyong intranet. It is developed from a version of Mozilla Firefox and is distributed with the Linux-based operating system Red Star OS that North Korea developed due to licensing and security issues with Microsoft Windows.

As the WikiPedia article indicates, the current version of the browser is **3.5** therefore the version number seen on the screenshot (*3.5b4*) is likely accurate. Based on the information we can construct a fairly comprehensive User-Agent string:

```
(X11, Linux i686) Geck/20130508 Fedora NaenaraBrowser/3.5b4
```

The above is the same string as I found on the following site that provides a fuller User-Agent information for the Naenara browser:

* https://developers.whatismybrowser.com/useragents/explore/software_name/naenara

Answer for this section: **Naenara 3.5b4**

## What Operating System and OS version did they use?
The WikiPedia article for the browser itself eludes to that this runs on an operating system called Red Star. This has its own wiki article: [Red Star OS](https://en.wikipedia.org/wiki/Red_Star_OS). From this we learn that this runs on Fedora, which tallies up with the OS information we've seen on the screenshot. 

Additional resources for the OS can be found below:

* https://archiveos.org/redstar/
* https://factrepublic.com/facts/22606/
* https://pastebin.com/cHAzyTE7
* https://www.northkoreatech.org/2020/02/11/red-star-4-appears-in-a-workplace-learning-system/

While the screenshot isn't entirely clear as to the version of the OS, the resources I found indicate that Red Star OS is currently on version 4 as the latest version. Version 3 is mentioned in a couple of places in the screenshot, which could be related to both the browser and the underlying OS or just the browser. It's a pretty safe bet that it will be most likely Red Star OS 3.

Answer for this section: **Red Star 3 (released ~2012) or Red Star 4 (released late 2017)**

## What is notable about this OS?
Where do we begin? The OS appears to be as oppressive as the regime that has developed it. 

> https://www.theregister.com/2015/12/29/north_korea_red_star_os/
> It was discovered in July that the software appends a fingerprint derived from the computer's hardware to files when they are opened.
> The antivirus scanner, scnprc, has a user interface, and cannot be disabled without provoking a system reboot. It has a particularly crucial file called /tmp/AnGae.dat. Apparently, "Angae" translates to "fog" in Korean.
>
> AnGae.dat contains UTF-16 strings of text in several different languages – phrases that, for example, translate into "strike with fists," "punishment," and “hungry". Any media files found by scnprc that contain any of the listed strings are automatically deleted.
>
> The watermarking service, opprc, runs in the background out of sight, unlike the antivirus.

> https://www.forensicxs.com/tag/naenara/
> The OS includes a securityd that mimics the one present in Mac OS and which features a function to validate the OS, integrity checking, and hardcoded MD5 checksums. The system calls the validate_os() function at startup and reboots if the process fails, which reveals that users are not allowed to make modification to the platform’s core capabilities

> https://www.fastcompany.com/3036046/what-its-like-to-use-north-koreas-red-star-os
> “In the desktop wallpapers folder you have pictures of the North Korean countryside, but with artillery cannons peppered across the hillsides. And the cannons all looked the same. They’ve clearly been Photoshopped in,” says Bowerman. “Then there’s one with a shot of a beautiful Pyongyang lit up at night with soft lights on snowy-perfect streets. But in reality this is a scene you would almost certainly never see.”

Answer for this section: **The OS watermarks files on the system with the user's MAC address to track users and the files they are interacting with. Propaganda from calendaras to wallpapers are among some more of the notable peculiarities for this OS**

### Additional resources
I figured I would add some more resources I came across while researching this challenge:

Browser:
* https://dbpedia.org/page/Naenara_(browser)
* https://thadafinser.github.io/UserAgentParserComparison/v5/user-agent-detail/67/18/67188569-9293-4a76-927b-4162b66345c9.html
* https://github.com/danielmiessler/SecLists/blob/master/Fuzzing/User-Agents/software-name/naenara.txt
* https://web.archive.org/web/20151215201456/http://blog.whitehatsec.com/north-koreas-naenara-web-browser-its-weirder-than-we-thought/
* https://www.youngpioneertours.com/naenara-browser/

Operating System:
* https://thenextweb.com/news/hands-north-koreas-homegrown-operating-system-red-star
* https://www.extremetech.com/computing/219963-north-koreas-linux-based-red-star-os-is-as-oppressive-as-youd-expect
* https://gamelust.com/news/investigation-steam-account-north-korea/
