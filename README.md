## Introduction

Alter is a Trezor alternative, powered by a recently awarded “Digital Public Goods Alliance” by UNICEF, Fedora Linux 35 (an open source operating sys-
tem based on Linux kernel) and other third party components, complimented manually written software.

The primary goal of Alter is to decrease the risks of being hacked, and provide a secure and private container for the user data, for people who doesn't have time to deal with every setups needed to do, through the use of an open source software, whereas the user can review the source code, thus being able modify it based on their preference.

However, despite all the modification, Alter is not a hack proof device, it still can be hacked, especially on the internet, depending from the client side, as once it was handled to the client, the device is fully modifiable upto a degree where it can lose all its security or secure it to a degree where it is unusable.

Quoting [Arch Linux Wiki](https://wiki.archlinux.org/title/security) :

> It is possible to tighten security to the point where the system is unusable.

## Device Mechanism

The device contained content access phase is consisted of 3 stages, (1.) Decryption of LUKS2 system encryption using master password, (2.) User account access from GDM (GNOME Display Manager), and (3.) Access of user content using the 24-key passphrase emailed to the user. [Refer to the PDF for the details](https://raw.githubusercontent.com/iaacornus/sys/devel/manscript/alter_patent_ppr_main.pdf).

Stage 1, has no trial limit, therefore the user can try as much as they can in decryption process of the system, this also applies to the stage 2. 

However in stage 3, the system has strict measures, as this is the last measure in data breach prevention. In stage 3, the user has 3 trials every access. Whereas, in every failed attempts, the system regenerates a new 24-key passphrase and sends it again to the registered email. If the 3 trials failed, the system will backup all user data and compress it into tar.gz format and email it into the user, and render the system unusable, where it can be reformatted again for it to be reused again.

## About the developer

The main developer and the author of the idea is James Aaron Erang, a 18 year old high school student from Philippines. The author has many experience from programming, computers and operating systems, especially Linux/GNU. Furthermore, he is also a student researcher in field of Biology, and he also utilizes computer science in his research studies.

[ResearchGate](https://www.researchgate.net/profile/James-Aaron-Erang) | [ORCID](https://www.researchgate.net/profile/James-Aaron-Erang) | jamesaaron2127@gmail.com
