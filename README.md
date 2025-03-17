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

![Screenshot 2025-03-17 160250](https://github.com/user-attachments/assets/e325f05b-ea2b-4779-8338-4d621a5fec38)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![Screenshot 2025-03-17 160630](https://github.com/user-attachments/assets/fb1dd9d3-94aa-4602-a479-556710cae17d)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![Screenshot 2025-03-17 160746](https://github.com/user-attachments/assets/cbaee241-19d4-44e6-a79f-1679c5a33b15)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![Screenshot 2025-03-17 160923](https://github.com/user-attachments/assets/1be42573-3040-4fd3-8177-1ce83e2dedf1)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![Screenshot 2025-03-15 014528](https://github.com/user-attachments/assets/38f79fa6-1d22-409e-9143-a5381da94e1f)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![Screenshot 2025-03-15 014658](https://github.com/user-attachments/assets/ceb3ef44-2188-4cf4-ae91-ee205bbce82a)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![Screenshot 2025-03-15 021548](https://github.com/user-attachments/assets/a814b77f-37eb-43c1-9a41-ee9c094e3c9f)

 
# DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![WhatsApp Image 2025-03-15 at 09 08 17_0bf124b7](https://github.com/user-attachments/assets/93107171-3440-4fdc-99dd-a20b2964f85d)







## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:
![WhatsApp Image 2025-03-15 at 09 11 13_99bf18aa](https://github.com/user-attachments/assets/17b8a9cd-a5fa-4bb2-9131-01bbf9792026)


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


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![Screenshot 2025-03-17 164312](https://github.com/user-attachments/assets/0630835f-3433-41f2-af22-070ab8aa9c6c)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![smtp 2](https://github.com/user-attachments/assets/15114af7-33fd-4dcb-9804-e3b4bf468f59)

## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  
  ![WhatsApp Image 2025-03-15 at 09 14 33_04c656ee](https://github.com/user-attachments/assets/e83c81a0-4ae6-40cf-bd37-28995f058ac8)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![nmap](https://github.com/user-attachments/assets/634ca1a1-9d7a-4e99-bcd5-28f41c4ebd79)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

