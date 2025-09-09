\# 🛡️ Pi-hole Configuration \& Blocklists



!\[Pi-hole](https://img.shields.io/badge/Pi--hole-v5%2B-brightgreen?logo=pi-hole\&logoColor=white)

!\[Maintained](https://img.shields.io/badge/Maintained-Yes-blue)

!\[Lists](https://img.shields.io/badge/Blocklists-30-red)



This repository contains my personal \*\*Pi-hole configuration\*\* and curated \*\*blocklists\*\*.  

It’s designed to provide \*\*network-wide ad blocking\*\*, \*\*privacy protection\*\*, and \*\*malware defense\*\*.  



---



\## ✨ Features

✅ Blocks ads, trackers, and telemetry across the entire network  

✅ Protects against phishing, malware, and crypto-miners  

✅ Includes optional lists for adult sites, fake news, gambling, and regional ads  

✅ Uses \*\*OISD\*\* + \*\*HaGeZi\*\* as core sources for high coverage \& low false-positives  

✅ Easy to import and update with `pihole -g`  



---



\## 📂 Blocklists Overview



| Category        | Lists Used |

|-----------------|------------|

| 📰 \*\*General Ads \& Trackers\*\* | StevenBlack, AdAway, AdGuard, Admiral, EasyPrivacy, AnudeepND, GoodbyeAds, WaLLy3K |

| 🛡️ \*\*Security \& Malware\*\* | Prigent (Ads \& Malware), CyberCrime Tracker, Dandelion Sprout Anti-Malware, URLHaus, HaGeZi Pro++, HaGeZi TIF |

| 🔒 \*\*Privacy\*\* | WindowsSpyBlocker, Disconnect.me Tracking, Perflyst Android Tracking, NoTracking |

| 🎯 \*\*Niche / Special\*\* | Facebook \& Instagram Tracking, Phishing Army, APWG Phishing, NoCoin, EasyList China \& Germany |

| 🚫 \*\*Content Filtering\*\* | Sinfonietta Porn Block, StevenBlack Fake News + Gambling |



---



\## 📜 Full Blocklist Set



<details>

<summary>Click to expand (30 lists)</summary>



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

21\. \[APWG Phishing](https://raw.githubusercontent.com/mitchellkrogza/Phishing.Database/master/phishing-domains-ACTIVE.txt)  

22\. \[NoCoin Miner Protection](https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/hosts.txt)  

23\. \[EasyList China](https://easylist-downloads.adblockplus.org/easylistchina.txt)  

24\. \[EasyList Germany](https://easylist-downloads.adblockplus.org/easylistgermany.txt)  

25\. \[Sinfonietta Porn Block](https://raw.githubusercontent.com/Sinfonietta/hostfiles/master/pornography-hosts)  

26\. \[Disconnect.me Tracking](https://s3.amazonaws.com/lists.disconnect.me/simple\_tracking.txt)  

27\. \[StevenBlack Fake News + Gambling](https://raw.githubusercontent.com/StevenBlack/hosts/master/alternates/fakenews-gambling/hosts)  

28\. \[URLHaus Malware](https://urlhaus.abuse.ch/downloads/hostfile/)  

29\. \[HaGeZi Pro++](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/hosts/pro.plus.txt)  

30\. \[HaGeZi TIF Aggregation](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/hosts/tif.txt)  



</details>



---



\## ⚙️ Setup



Clone this repo on your Pi-hole server:



```bash

cd /etc/pihole

git clone https://github.com/rhshourav/pi-hole.git pihole-config



