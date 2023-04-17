# Assignment: Deploy and monitor honeypot
### Date: 21NOV2021

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.


### MHN-Admin Deployment
**Summary:** How did you deploy it? Did you use GCP, AWS, Azure, Vagrant, VirtualBox, etc.?

	I deployed the MHN-Admin server vm and the honeypot hosts using Google Cloud and the instructions provided. 

![MHN-admin installed](https://user-images.githubusercontent.com/10326824/140461678-d829db99-82d4-4cdb-ba93-cce090bdcf88.gif)



### Dionaea Honeypot Deployment

**Summary:** Briefly in your own words, what does dionaea do?

	Dionaea is software that can be installed on a computer and aims to make the host computer vulnerable on purpose 
	this in an effort to make the host attractive to attackers on the internet (by simulating open ports and vulnerable software) 
	all in an effort to capture malware or attack methodology signatures. The installed Dionaea sensor works with MHN 
	(which acts as the portal) to observe/log the attacks that targeted the vulnerable host.

![Dionaea Deployed](https://user-images.githubusercontent.com/10326824/140461763-f820d351-3255-4226-9c8a-e6e670480030.gif)


### Database Backup

**Summary:** What is the RDBMS that MHN-Admin uses? What information does the exported JSON file record?

	MHN-Admin uses MongoDB as its database for keeping sensor logs. 
	The session.json file exported is a log of the sensors deployed with MHN. The log file includes
	protocol, timestamp, source ip, destination ip, protocol name, identifier and honeypot name.

*Be sure to upload session.json directly to this GitHub repo/branch in order to get full credit.*


### Deploying Additional Honeypot(s)
#### anum honeypot and conpot honeypot


**Summary:** What does this honeypot simulate and do for a security researcher?

	Conpot sensor that can be be easily configured to simulates industrial control systems.
	Like dionaea, anum is a honeypot that follows the concepts of Nepenthes.
	
	The honeypots simulate vulnerable/exposed computers on the internet and allows security 
	researchers to deploy clients out on the internet and learn/analyze the software and methods malicious actors on the internet are using. 

![Deploying Additional POTs](https://user-images.githubusercontent.com/10326824/140461812-c4498a87-3528-4297-a0c9-b232b50e8377.gif)



### Malware Capture and Identification
#### Malware:: Ransom:Win32/CVE-2017-0147.b52e707a


**Summary:** How did you find it? Which honeypot captured it? What does each malware do?
	The MHN server log showed several payloads in the payloads tap.
	
	This malware was found by the dionaea honeypot. 
	
	The malware targets the WannaCry vulnerability in SMBv1 server in Microsoft Windows Vista SP2; 
	Windows Server 2008 SP2 and R2 SP1; Windows 7 SP1; Windows 8.1; Windows Server 2012 Gold and R2; 
	Windows RT 8.1; and Windows 10 Gold, 1511, and 1607; and Windows Server 2016


MD5 Hash::	8b7137adb7aac5cbf55b039babb612bc

SHA1 Hash::	969ffdc09c2ff058e040120824eae8e796bead9cfc7549b44704944bfa8d0731a70bc94cd34ad5e1c3a254ce07d212a9ae60f958b64243d0ec7c75b9f6fe554f

![IdentifyingMalware](https://user-images.githubusercontent.com/10326824/140461882-ce16d8da-0c1e-4fc2-9cde-6d8e968f8eb9.gif)


## Notes
Describe any challenges encountered while doing the assignment.
