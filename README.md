# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
![etht exp3,1](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/4ab39462-0868-4302-8000-186656a332c5)



filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![etht exp3,2](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/3381e402-651b-46c5-82ae-f33ccf78f906)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![etht exp3,3](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/4dee2347-8ef1-444e-942c-cbb229d7d143)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![etht exp3,4](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/94005ce1-d13a-4af7-b717-ff1b4bbb669f)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![etht exp3,5](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/c272d806-9f9f-4d15-a8f5-31396634b4d7)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![etht exp3,6](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/ea7c7133-2dce-4cc8-81b0-ff3c22c0a813)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![etht exp3,7](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/15c583ab-e84f-4fae-8083-575177b07939)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![etht exp3out1](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/483a9d90-4cdd-40c9-b542-d2fd4913366a)

![etht exp3out2](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/6a6e2ec4-a1f6-4610-b463-3655d8806cd6)




##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
![etht exp3out3](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/8daedf03-b923-42a7-8659-17bc4ce98c59)



##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![etht exp3out4](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/a1fffeea-3007-40f9-95de-230a54121152)


select any username in the first column of the above file and check the same
![image](https://github.com/AasrithSairam/Enumeration/assets/139331438/bfca1263-569a-4115-be65-e54c3a6a63e8)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
 
![etht exp3out5](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/4e8772d9-4b19-4fd3-8f15-9ed19746ff7f)
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![etht exp3out6](https://github.com/SVENGADAKRISHNAN/Enumeration/assets/147473084/f0ae79a3-b006-41df-9134-6c3de6660e49)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

