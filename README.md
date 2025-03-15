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
Following searches for all the sites that is in the domain linkedin.com
![image](https://github.com/user-attachments/assets/fe7556d7-cdfe-4d23-b511-e770f66cba4f)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain linkedin.com
![image](https://github.com/user-attachments/assets/813b345c-8347-4a0c-8122-87f7fccd3b72)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![image](https://github.com/user-attachments/assets/bddf317e-6998-4200-9a75-8a6236bbb291)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:Hafeezul" would search for pages that contain the word "admin" within the URL.
![image](https://github.com/user-attachments/assets/473d2d6c-ff46-4d7b-918f-cce3299c5894)




intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:Networkchuck of" would search for pages that contain "index of" within the title tag.
![image](https://github.com/user-attachments/assets/c0744c28-4516-4419-b7ad-9e091f933bc7)




link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/user-attachments/assets/42ed29de-aa76-443e-be0d-c13a3740014c)




cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/user-attachments/assets/9d0a94dc-c3b9-470a-b9d1-79c8357d2572)



 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![Screenshot 2025-03-15 140526](https://github.com/user-attachments/assets/f777f506-cdba-40f9-abcf-d57941789e90)







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
##OUTPUT:
![Screenshot 2025-03-15 140827](https://github.com/user-attachments/assets/43e91f2f-551e-4f95-9156-ad3bedea8f9b)



##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
##OUTPUT:
![image](https://github.com/user-attachments/assets/bc40aae1-2b65-4d7a-a523-b321dedd0614)





In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:



select any username in the first column of the above file and check the same
##OUTPUT
![image](https://github.com/user-attachments/assets/b04ba701-00bb-40e2-9ff5-62d52d949618)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands  
 ##Output
 ![image](https://github.com/user-attachments/assets/f8bbe197-faf5-4a7e-84be-9c152af71a1c)

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
## OUTPUT:
![image](https://github.com/user-attachments/assets/a091376a-bf43-40c1-bfcd-bfb4d05bb166)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

