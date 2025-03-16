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
![Screenshot 2025-03-15 131946](https://github.com/user-attachments/assets/35e39e75-eaed-4feb-b4c0-7e5203a1950c)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![Screenshot 2025-03-15 132022](https://github.com/user-attachments/assets/c75c4c8c-46d0-42e6-9ec8-1b4e5f636706)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.![Screenshot 2025-03-15 132101](https://github.com/user-attachments/assets/eb76479f-14ee-4176-96df-09ef2cacd450)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![Screenshot 2025-03-15 132145](https://github.com/user-attachments/assets/4193a3a8-7033-4860-b571-c6a2c2a9e99e)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![Screenshot 2025-03-15 132244](https://github.com/user-attachments/assets/78402874-17e4-47ad-be7f-a385f06fea66)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.![Screenshot 2025-03-15 132331](https://github.com/user-attachments/assets/06e930f3-4da6-4345-a82f-0b35e75cf476)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 ![Screenshot 2025-03-15 133711](https://github.com/user-attachments/assets/ee3fd5a0-a93d-4c35-bfdc-3809a1caac0a)

#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:



![Screenshot 2025-03-15 142604](https://github.com/user-attachments/assets/b44f32a1-6404-4989-b91f-1f9b08cd4822)






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


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![Screenshot 2025-03-15 141048](https://github.com/user-attachments/assets/7cff3776-3eaa-40c0-8d2a-0338c4785932)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![Screenshot 2025-03-15 143211](https://github.com/user-attachments/assets/2d034559-610d-4e55-949b-b23acbb1f22f)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
![Screenshot 2025-03-15 142628](https://github.com/user-attachments/assets/13fc3f91-e761-4c9b-a1a8-c24df5c687a2)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![Screenshot 2025-03-15 143312](https://github.com/user-attachments/assets/674f1fd4-2769-4d36-84e3-64780ca9e665)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

