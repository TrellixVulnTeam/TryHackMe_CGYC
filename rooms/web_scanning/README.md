# Web Scanning

#Date: 18.09.2020

IP:`10.10.179.32`

----------
# [Nikto cheatsheet](https://redteamtutorials.com/2018/10/24/nikto-cheatsheet/)
```
sinq@kali:~/TryHackMe/web_scanning$ nikto -h 10.10.179.32
- Nikto v2.1.6
---------------------------------------------------------------------------
+ Target IP:          10.10.179.32
+ Target Hostname:    10.10.179.32
+ Target Port:        80
+ Start Time:         2020-09-18 18:09:13 (GMT2)
---------------------------------------------------------------------------
+ Server: Apache/2.4.7 (Ubuntu)
+ Retrieved x-powered-by header: PHP/5.5.9-1ubuntu4.26
+ The anti-clickjacking X-Frame-Options header is not present.
+ The X-XSS-Protection header is not defined. This header can hint to the user agent to protect against some forms of XSS
+ The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type
+ Cookie PHPSESSID created without the httponly flag
+ Root page / redirects to: login.php
+ No CGI Directories found (use '-C all' to force check all possible dirs)
+ Apache/2.4.7 appears to be outdated (current is at least Apache/2.4.37). Apache 2.2.34 is the EOL for the 2.x branch.
+ OSVDB-3268: /config/: Directory indexing found.
+ /config/: Configuration information may be available remotely.
+ OSVDB-3268: /docs/: Directory indexing found.
+ OSVDB-3233: /icons/README: Apache default file found.
+ /login.php: Admin login page/section found.
+ 7889 requests: 0 error(s) and 11 item(s) reported on remote host
+ End Time:           2020-09-18 18:18:24 (GMT2) (551 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested
```


---------
# OWASP-zap

GUI tool, less fun that Nikto



