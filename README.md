# Week10and11Assign
Week 10 &amp; 11 Project: Honeypot

# Honeypot Assignment

**Time spent:** **6** hours spent in total

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.


### MHN-Admin Deployment (Required)
**Summary:** How did you deploy it? Did you use GCP, AWS, Azure, Vagrant, VirtualBox, etc.?

	I deployed the MHN-Admin server vm and the honeypot hosts using Google Cloud and the instructions provided. 
	
<img src="mhn-admin.gif">


### Dionaea Honeypot Deployment (Required)


**Summary:** Briefly in your own words, what does dionaea do?

Dionaea is a piece of software can be installed on a computer that aims to make the host computer vulnerable on purpose
this in an effort to the host attractive to attackers on the internet (by simulating open ports and vulnerable software) in 
an effort to capture malware or attack methodology signatures. Our walked through install of Dionaea works with 
MHN (which acts as the portal) observe/analyze the attacks that targeted the vulnerable host.

<img src="dionaea-honeypot.gif">


### Database Backup (Required) 

**Summary:** What is the RDBMS that MHN-Admin uses? What information does the exported JSON file record?
*Be sure to upload session.json directly to this GitHub repo/branch in order to get full credit.*


### Deploying Additional Honeypot(s) (Optional)
#### X Honeypot



**Summary:** What does this honeypot simulate and do for a security researcher?
This honeypot simulate vulnerable/exposed computers on the internet and allows security researchers
to deploy clients out on the internet and learn/analyze the software and methods malicious actors on the internet 
are using. 


<img src="x-honeypot.gif">
### Malware Capture and Identification (Optional)
#### X Malware


**Summary:** How did you find it? Which honeypot captured it? What does each malware do?
MD5 Hash: *Run `md5sum` on the file and record the hash here.*
SHA1 Hash: *Run `sha1sum` on the file and record the hash here.*
<img src="x-malware.gif">


## Notes
Describe any challenges encountered while doing the assignment.![image](https://user-images.githubusercontent.com/10326824/140461522-87b2f834-c03e-4e02-a2af-95c5978d50cf.png)
