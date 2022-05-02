 
nmap-port-scanautomation - Auto NMAP Scanning Script
============================================



Developed by Resikesh M R

https://github.com/RESIKESH/nmap-port-scanautomation/

Released under AGPL see LICENSE for more information

Installing  
=======================
    git clone https://github.com/RESIKESH/nmap-port-scanautomation/


How To Use	
=======================
    ./portmap.sh


Features	
=======================

* Discovers live devices
* Auto launches port scans on only the discoverd live devices
* Can run mulitple instances on multiple adaptors at once
* Creates client Ref directory for each scan
* Outputs all unique open ports in a Nessus ready format. Much faster to scan in Nessus.
* Runs as default a T4 speed scan. If you find this too slow, you can press CTRL C in the scan window and it will cleanup and relaunch that one scan with T5 speed option.
* Logs all start/stop times, live hosts, hosts down, unique ports.
* Auto creates a custom Nessus policy with only the discovered ports, must faster to scan. *

* * Read the script header carefully, in order for the auto Nessus policy creater you must first save a default template to the same directory as the script. The script will detect the default template and create you a unique Nessus policy after each scan for just the unique ports. Then simply import the policy into Nessus and scan just the live devices that the  script found. This will save a massive amount of time scanning, plus will give you more accurate findings.

* * By Default it will scan a full TCP, Quick UDP, Common ports and a Safe Script scan. You can turn these on and off in the header. 

Requirements   
=======================
* NMAP http://www.nmap.org

Tested on Backtrack 5 and Kali.




Change Log
=======================

Version 1.8 - Official release.
