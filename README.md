# Enumeration

# Explore Google hacking and enumeration :

# AIM :

To use Google for gathering information and perform enumeration of targets.

## PROCEDURE :

### STEP 1 :

Install kali linux either in partition or virtual box or in live mode.

### STEP 2 :

Investigate on the various Google hacking keywords and enumeration tools as follows:

### STEP 3 :

Open terminal and try execute some kali linux commands.

## Pen Test Tools Categories :  

Following Categories of pen test tools are identified:

 Information Gathering.

### Google Hacking :

  Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking :

#### site : 

  This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain youtube.com

![h1](https://github.com/Vishwarathinam/Enumeration/assets/95266350/a2c78d4c-9974-48a0-8ce8-48782ab6d5f5)


##### filetype : 

  This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain youtube.com

![h2](https://github.com/Vishwarathinam/Enumeration/assets/95266350/3cb77175-dd92-48cf-8f4e-11670caeca49)


#### intext : 

  This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![h3](https://github.com/Vishwarathinam/Enumeration/assets/95266350/2a541497-c5d5-4007-8d35-9f82c262a4b2)



#### inurl : 

  This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
  ![h4](https://github.com/Vishwarathinam/Enumeration/assets/95266350/b00d1806-1145-42ca-807a-8aec9178eba2)



#### intitle :

  This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![h5](https://github.com/Vishwarathinam/Enumeration/assets/95266350/2bc77918-9452-4415-bc98-6a4c11291854)


#### link :

  This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![h6](https://github.com/Vishwarathinam/Enumeration/assets/95266350/f7d493bb-cd52-4f84-a95d-780cca76c1d5)


#### cache : 

  This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![h7](https://github.com/Vishwarathinam/Enumeration/assets/95266350/1f755997-00f6-4817-8c53-0677e0651622)


# DNS Enumeration :

## DNS Recon :

Provides the ability to perform:

Check all NS records for zone transfers

Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)

Perform common SRV Record Enumeration

Top level domain expansion

## OUTPUT :
![h8](https://github.com/Vishwarathinam/Enumeration/assets/95266350/c1cbc8a0-c2f3-4ed0-9e6a-1ee35f6fab41)

![h9](https://github.com/Vishwarathinam/Enumeration/assets/95266350/695b3665-064f-4f8f-ad93-13dfe8c80e78)


## dnsenum :

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

![h10](https://github.com/Vishwarathinam/Enumeration/assets/95266350/4a6dd3c7-b3fe-4990-8bc2-ac357e767cb4)



## smtp-user-enum :

  Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
  
![h11](https://github.com/Vishwarathinam/Enumeration/assets/95266350/f2d65a9c-4b02-4d62-9b77-f68bb9f5a2bd)



  In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![h12](https://github.com/Vishwarathinam/Enumeration/assets/95266350/f2d8bd1f-95a1-4759-b425-3cbc5485de4d)



  Select any username in the first column of the above file and check the same
  
![h13](https://github.com/Vishwarathinam/Enumeration/assets/95266350/65c05661-867a-4b1c-a494-9979ea717895)



# Telnet for smtp enumeration :

Telnet allows to connect to remote host based on the port no. For smtp port no is 25

telnet <host address> 25 to connect

and issue appropriate commands.
  
## Output :

![h14](https://github.com/Vishwarathinam/Enumeration/assets/95266350/536ef3ad-2ad7-42fc-9cbf-9b47cd5f9470)



## nmap –script smtp-enum-users.nse <hostname> :

  The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT :

![h15](https://github.com/Vishwarathinam/Enumeration/assets/95266350/e96b9e1b-8d7a-4dd8-a254-90f48e1fc0a6)



## RESULT :

The Google hacking keywords and enumeration tools were identified and executed successfully.
