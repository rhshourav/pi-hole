# 🛡️ Pi-hole Configuration & Blocklists

![Pi-hole](https://img.shields.io/badge/Pi--hole-v5%2B-brightgreen?logo=pi-hole&logoColor=white)  
![Maintained](https://img.shields.io/badge/Maintained-Yes-blue)  
![Blocklists](https://img.shields.io/badge/Blocklists-31+-red)  
![Updates](https://img.shields.io/badge/Auto--Update-Every%205h-orange)  

This repository contains my **Pi-hole configuration** and carefully curated **blocklists**.  
It’s optimized for **network-wide ad blocking**, **privacy protection**, and **malware defense** with minimal false positives.  

---

## ✨ Features
- ✅ Blocks ads, trackers, and telemetry across all devices  
- 🛡️ Shields against phishing, malware, and cryptominers  
- 🎯 Optional filters for adult sites, gambling, fake news & regional ads  
- ⚡ Uses **OISD** + **HaGeZi** for maximum coverage with low breakage  
- 🔄 Automatically refreshed every 5 hours with `pihole -g`  

---

## 📂 Blocklist Categories

### 📰 General Ads & Trackers
- [StevenBlack Unified](https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts)  
- [AdAway](https://adaway.org/hosts.txt)  
- [AdGuard](https://v.firebog.net/hosts/AdguardDNS.txt)  
- [AdGuard DNS Filter](https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt)  
- [Admiral](https://v.firebog.net/hosts/Admiral.txt)  
- [EasyPrivacy](https://v.firebog.net/hosts/Easyprivacy.txt)  
- [AnudeepND Adservers](https://raw.githubusercontent.com/anudeepND/blacklist/master/adservers.txt)  
- [GoodbyeAds (Mobile)](https://raw.githubusercontent.com/jerryn70/GoodbyeAds/master/Hosts/GoodbyeAds.txt)  
- [WaLLy3K (w3kbl)](https://v.firebog.net/hosts/static/w3kbl.txt)  

---

### 🛡️ Security & Malware Protection
- [Prigent Ads](https://v.firebog.net/hosts/Prigent-Ads.txt)  
- [Prigent Malware](https://v.firebog.net/hosts/Prigent-Malware.txt)  
- [CyberCrime Tracker](https://cybercrime-tracker.net/all.php)  
- [Dandelion Sprout Anti-Malware](https://raw.githubusercontent.com/DandelionSprout/adfilt/master/Alternate%20versions%20Anti-Malware%20List/AntiMalwareHosts.txt)  
- [URLHaus Malware](https://urlhaus.abuse.ch/downloads/hostfile/)  
- [HaGeZi Pro++](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/hosts/pro.plus.txt)  
- [HaGeZi TIF Aggregation](https://raw.githubusercontent.com/hagezi/dns-blocklists/main/hosts/tif.txt)  

---

### 🔒 Privacy & Telemetry
- [WindowsSpyBlocker](https://raw.githubusercontent.com/crazy-max/WindowsSpyBlocker/master/data/hosts/spy.txt)  
- [Disconnect.me Tracking](https://s3.amazonaws.com/lists.disconnect.me/simple_tracking.txt)  
- [Perflyst Android Tracking](https://raw.githubusercontent.com/Perflyst/PiHoleBlocklist/master/android-tracking.txt)  
- [NoTracking](https://raw.githubusercontent.com/notracking/hosts-blocklists/master/domains.txt)  

---

### 🎯 Niche / Special Purpose
- [Facebook & Instagram Tracking](https://raw.githubusercontent.com/jmdugan/blocklists/master/corporations/facebook/all)  
- [Phishing Army](https://phishing.army/download/phishing_army_blocklist_extended.txt)  
- [APWG Phishing](https://raw.githubusercontent.com/mitchellkrogza/Phishing.Database/master/phishing-domains-ACTIVE.txt)  
- [NoCoin Miner Protection](https://raw.githubusercontent.com/hoshsadiq/adblock-nocoin-list/master/hosts.txt)  
- [EasyList China](https://easylist-downloads.adblockplus.org/easylistchina.txt)  
- [EasyList Germany](https://easylist-downloads.adblockplus.org/easylistgermany.txt)  

---

### 🚫 Content Filtering (Optional)
- [Sinfonietta Pornography Block](https://raw.githubusercontent.com/Sinfonietta/hostfiles/master/pornography-hosts)  
- [StevenBlack Fake News + Gambling](https://raw.githubusercontent.com/StevenBlack/hosts/master/alternates/fakenews-gambling/hosts)  

---

## ⚡ Installation

Import the blocklists into Pi-hole with:

```bash
pihole -g
```

### ⏰ Automatic Updates (Cron Setup)
To keep your blocklists up to date every 5 hours, configure a cron job:

1. Open the root crontab:
```bash
sudo crontab -e
```

2. Add the following line:
```bash
0 */5 * * * /usr/local/bin/pihole -g > /dev/null 2>&1
```

Save & exit.
Cron will now run pihole -g at 00:00, 05:00, 10:00, 15:00, and 20:00 daily.
