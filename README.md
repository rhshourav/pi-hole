\# Pi-hole Configuration Repository



This repository contains my personal \*\*Pi-hole configuration\*\*, blocklists, and related setup notes.  

It’s designed to provide \*\*network-wide ad-blocking\*\*, \*\*privacy protection\*\*, and \*\*malware defense\*\* using a curated collection of DNS blocklists.



---



\## 📌 Contents

\- `adlists.list` → curated blocklists for Pi-hole

\- Configuration notes \& tweaks

\- References to additional resources



---



\## 🚀 Features

\- \*\*Comprehensive Ad Blocking\*\* → removes ads across websites, apps, and streaming platforms  

\- \*\*Privacy Protection\*\* → blocks trackers, telemetry, and analytics domains  

\- \*\*Security Hardening\*\* → includes anti-phishing, anti-malware, and crypto-miner blocklists  

\- \*\*Regional \& Niche Lists\*\* → optional lists for region-specific ads, adult content, fake news, gambling, and social media tracking  

\- \*\*Optimized Selection\*\* → avoids unnecessary overlap by using strong, well-maintained sources (OISD, HaGeZi, StevenBlack, Firebog, etc.)



---



\## 📂 Blocklists in Use

Here’s the full list of enabled sources:



1\. \[StevenBlack Unified](https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts)  

2\. \[AdAway](https://adaway.org/hosts.txt)  

3\. \[PolishFiltersTeam](https://raw.githubusercontent.com/PolishFiltersTeam/KADhosts/master/KADhosts.txt)  

4\. \[FadeMind Spam Hosts](https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.Spam/hosts)  

5\. \[WaLLy3K w3kbl](https://v.firebog.net/hosts/static/w3kbl.txt)  

6\. \[AdGuard](https://v.firebog.net/hosts/AdguardDNS.txt)  

7\. \[Admiral](https://v.firebog.net/hosts/Admiral.txt)  

8\. \[EasyPrivacy](https://v.firebog.net/hosts/Easyprivacy.txt)  

9\. \[Prigent Ads](https://v.firebog.net/hosts/Prigent-Ads.txt)  

10\. \[AnudeepND Adservers](https://raw.githubusercontent.com/anudeepND/blacklist/master/adservers.txt)  

11\. \[OISD Full](https://big.oisd.nl/)  

12\. \[WindowsSpyBlocker](https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt)  

13\. \[GoodbyeAds (Mobile)](https://raw.githubusercontent.com/jerryn70/GoodbyeAds/master/Hosts/GoodbyeAds.txt)  

14\. \[Prigent Malware](https://v.firebog.net/hosts/Prigent-Malware.txt)  

15\. \[CyberCrime Tracker](https://cybercrime-tracker.net/all.php)  

16\. \[NoTracking](https://raw.githubusercontent.com/notracking/hosts-blocklists/master/domains.txt)  

17\. \[Dandelion Sprout Anti-Malware](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Alternate%20versions%20Anti-Malware%20List/AntiMalwareHosts.txt)  

18\. \[Perflyst Android Tracking](https://raw.githubusercontent.com/Perflyst/PiHoleBlocklist/master/android-tracking.txt)  

19\. \[Facebook \& Instagram Tracking](https://raw.githubusercontent.com/jmdugan/blocklists/master/corporations/facebook/all)  

20\. \[Phishing Army](https://phishing.army/download/phishing\_army\_blocklist\_extended.txt)  

21\. \[Anti-Phishing Working Group](https://raw.githubusercontent.com/mitchellkrogza/Phishing.Database/master/phishing-domains-ACTIVE.txt)  

22\. \[NoCoin Miner Protection](https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/hosts.txt)  

23\. \[EasyList China](https://easylist-downloads.adblockplus.org/easylistchina.txt)  

24\. \[EasyList Germany](https://easylist-downloads.adblockplus.org/easylistgermany.txt)  

25\. \[Sinfonietta Pornography Block](https://raw.githubusercontent.com/Sinfonietta/hostfiles/master/pornography-hosts)  

26\. \[Disconnect.me Tracking](https://s3.amazonaws.com/lists.disconnect.me/simple\_tracking.txt)  

27\. \[StevenBlack Fake News + Gambling](https://raw.githubusercontent.com/StevenBlack/hosts/master/alternates/fakenews-gambling/hosts)  

28\. \[URLHaus Malware](https://urlhaus.abuse.ch/downloads/hostfile/)  

29\. \[HaGeZi Pro++](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/hosts/pro.plus.txt)  

30\. \[HaGeZi TIF Aggregation](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/hosts/tif.txt)  



---



\## ⚙️ Usage

Clone this repo to your Pi-hole server and import the blocklists:



```bash

cd /etc/pihole

git clone https://github.com/rhshourav/pi-hole.git pihole-config



