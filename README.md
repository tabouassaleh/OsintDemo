# OsintDemo
Basic Info
* https://who.is/

Bing reverse ip (Demo)
* ip:176.65.66.66 

yahoo advanced search (Demo)
* http://search.yahoo.com/search/options?fr=%20fp-top&p= 

yandex advance search (Demo)
* http://www.yandex.com/search/advanced?&lr=10558 D

Subdomain Enum: (Demo)
* Manual site: and -
* http://www.google.com/advanced_search
* https://dnsdumpster.com/
* https://searchdns.netcraft.com/
* https://www.robtex.com/
* http://viewdns.info/reversewhois/
* https://www.yougetsignal.com/tools/web-sites-on-web-server/
* https://domainbigdata.com/
* http://www.wolframalpha.com/
* https://www.virustotal.com/#/home/search


ASN Approach (Demo)
* https://bgp.he.net (ASN:Autonomous System Number to get ip blocks)
* https://mxtoolbox.com/supertool.aspx 

Technology Approach (Demo)
* https://www.shodan.io/
* https://censys.io/
* https://www.zoomeye.org

Aquisition Approach (Demo)
* google
* wiki
* https://www.crunchbase.com

Old buggy link approach (Demo)
* google site: tools custom date

Darknet (Demo)
* https://ahmia.fi/
* http://grams7enufi7jmdl.onion.to/

Github recon (Demo)
* Creds, private keys etc
* https://github.com/techgaun/github-dorks


Now its getting boring so lets look at the tools
* https://github.com/aboul3la/Sublist3r  (uses multiple sources like google virus total)  (Demo)
* https://github.com/anshumanbh/brutesubs (Paralally runs multiple tools )
* https://github.com/TheRook/subbrute (bruteforce the subdomain)
* https://github.com/blechschmidt/massdns
* https://github.com/infosec-au/altdns (permutational approach)
* https://github.com/jfrancois/SDBF (smart dns bruteforcer)

subdomain takeover:
* https://github.com/nahamsec/HostileSubBruteforcer

To confirm still up we can use (Demo)
* https://github.com/ChrisTruncer/EyeWitness

Technology discovery (Demo)
* buildwith
* waplyzer

Content discovery
* Dirbuster
* https://github.com/OJ/gobuster

Lists for fuzzing
* https://github.com/danielmiessler/SecLists
* https://github.com/danielmiessler/RobotsDisallowed

Parameter Enum (Demo)
* https://github.com/maK-/parameth
* https://github.com/PortSwigger/backslash-powered-scanner/blob/master/resources/params

Link finder (searches links from js file) (Demo)
* https://github.com/GerbenJavado/LinkFinder

Vulns discovery (Demo)
* https://www.punkspider.org.      race360

Online scanners
* https://urlscan.io/
* https://asafaweb.com/

Social profile discovery etc
* https://inteltechniques.com/menu.html (username social profile etc)

Some other interesting things to look for
* Linkind for passive tech stack details via job posts, employee skills
* Search for 3rd party apps used 
* search for open jira instances
* search for devops setup puppet, chef, vagrant, ansible, jenkins
* search for open dev, staging envs


Intelligent attack with tools:

Recon-ng 

1. Domain name > email > wheather hacked or not by recon-ng

```
Discovery (Active recon with sending packet)
Exploitation (Using payload)
Import (to add list or prev projs)
Recon (passive recon)
Report (xml or html)

help
Workspaces
Workspaces list                        	to get the lists
Workspaces add osint
		
Keys list - to see which keys has been added
https://bitbucket.org/LaNMaSteR53/recon-ng/wiki/Usage%20Guide#!acquiring-api-keys

keys add bing_api testingggggggggggg
		
Show Modules 	(Take a domain and dig deeper)
use recon/domains-contacts/whois_pocs
		
Show info
set SOURCE abc.com
Run

Show dashboard - to see what we did so far
Show contacts - host table
		
Get credentials
use recon/contacts-credentials/hibp_paste

automate everyday workflow
record
resource
```

Maltego
* Maltego is an Open Source Intelligence application, which provides a platform to not only extract data but also to represent that data in a format which is easy to understand as well as analyze.


* Entity: An entity is a piece of data which is taken as an input to extract further information. E.g. domain name xyz.com

* Transform: A piece of code which takes an entity (or a group of entities) as an input and extracts data in the form of entity (or entities) based upon the relationship. E.g. DomainToDNSNameSchema: this transform will try to test various name schemas against a domain (entity).

* Machine: A machine is basically a set of transforms linked programmatically. E.g. Footprint L1: a transform which takes a domain as an input and generates various types of information related to the organization such as emails, AS number etc.


DataSploit:
* https://github.com/DataSploit/datasploit
* http://datasploit.info/

* https://hub.docker.com/r/appsecco/datasploit/
* https://hub.docker.com/r/ftorn/datasploit/
