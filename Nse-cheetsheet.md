
# **Nse-cheetsheet For Hackers:** 
Nse or Nmap Scripting Engine is a part of Nmap(Hacker tool) tool which is used by Pentesters,Bug hunters & Hackers to scan a network and then identify the vulnerbilities. So Here is a some special cheet codes or commands of Nse which can be used to exploit the web applications.

# **CheetSheet-Commands:**

* Nse command To identify Cookies Without Flags Bug:
  * nmap -p 443 --script http-cookie-flags <target> 

* Nse command For All CVE vulnerbilites: 
  * nmap -sV --script vulners [--script-args mincvss=<arg_val>] <target>

>
--------------------------------------------------------------------------------------------

* Nse command To check Whois Of Target: 
  * nmap --script whois-domain.nse <target>

* Nse command To Check WAF detecion Of Target: 
  * nmap --script=http-waf-fingerprint --script-args http-waf-fingerprint.intensive=1 <targets>

* Nse command To Brute Force Password Auditing Against Wordpress CMS/blog:
  * nmap -sV --script http-wordpress-brute <target>
  * nmap -sV --script http-wordpress-brute --script-args 'userdb=users.txt,passdb=passwds.txt,http-wordpress-brute.hostname=domain.com,http-wordpress-brute.threads=3,brute.firstonly=true' <target>
> I am not sure about this command that it will work or not.

* Nse To Enumerates Themes & Plugins Of Wordpress:
  * nmap -sV --script http-wordpress-enum <target>
  * nmap --script http-wordpress-enum --script-args check-latest=true,search-limit=10 <target>
  * nmap --script http-wordpress-enum --script-args type="themes" <target>

* Nse command To Identify XSS (Stored cross site script vulnerbilities): 
  * nmap -p80 --script http-stored-xss.nse <target>
> Again I m not sure.

* Nse command To Identify Cross domain policy vulnerbilites:
  * nmap --script http-cross-domain-policy <target>
  * nmap -p 80 --script http-cross-domain-policy --script-args http-cross-domain-policy.domain-lookup=true <target>

* Nse Command To Detects Cross Site Request Forgeries (CSRF) vulnerabilities: 
  * nmap -p80 --script http-csrf.nse <target>

* Nse command To Enumerates Drupal users by exploiting an information disclosure vulnerability:
  * nmap --script=http-drupal-enum-users --script-args http-drupal-enum-users.root="/path/" <targets>

* Nse command For Denial Of Service Attack:  
  * nmap --script http-slowloris --max-parallelism 400  <target>
> Again I m not sure.

* Nse command To check Denial Of Service Attack: 
  * nmap --script http-slowloris-check  <target>

* Nse command To retrive the server-status page for Apache webservers: 
  * nmap -sV --script http-apache-server-status <target>

* Nse command To Check For The HTTP Response Headers Related To Security(Strict Security not Enforced ) : 
  * nmap -p 443 --script http-security-headers <target>
