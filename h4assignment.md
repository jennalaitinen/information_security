# x) Read and summarize

A01:2021 - Broken Access Control
- Broken access control enforces that users cannot operate outside their permissions
- Some of the common access control vulnerabilities are bypassing access control checks, accessing API with missing access controls for POST, PUT and DELETE and Elevation of privilege
- Some things to help prevent accesss control: Disable web server directory listing and ensure file metadata, rate limit API and controller access to minimize the harm from automated attack tooling and reinforcing unique application businesss requirements
  
A05:2021 - Security Misconfiguration
- Security misfiguration can be identified by vulnerabilities including: unnecessary features that are enabled or installed, if the application is missing appropriate security hardening and if default accounts and their passwords are still enabled and unchanged
- You can prevent this by repeating a hardening process, sending security directivites and by an automated process to verify the effectiveness of the configurations and settings
- Example scenarios of attacks, this helps us visualize real-life scenarios and help us prepare for these
  
A06:2021 - Vulnerable and Outdated Components
- Some vulnerabilites are: software vulnerability by being unsupported or out-of-date, you are vulnerable if you don't scan your vulnerabilities reguarly and also if you don't secure the components' configurations
- You can prevent this by removing unused features, files and components. Also by only containing components from official sites and trustable sources and links
- Every organization must ensure an ongoing plan for monitoring, triaging, and applying updates or configuration changes for the lifetime of the application or portfolio

A03:2021 - Injection
- Vulnerabilities in an application are: when user-supplied data is not validated or filtered, when hostile data is being used directly or concatenated etc 
- preventing injection requires keeping data safe and separate from commands, this is done by: using a safe API that does not use the interpeter at all. Also using positive server-side input validation
- Example attack scenarios which include the commands, which makes it easy to observe and learn more.

Munroe: xkcd 327: Exploits of a Mom
- This page is a humour-based "comic" site
-  The "Exploits of a Mom" jokes about the mom naming her son something that when inserted into the computer, accidentally removes the student data from their computer ( https://xkcd.com/327/ )

# a) 
- Installation of Webgoat
    - I booted up my Linux and followed the commands and instructions on https://terokarvinen.com/2023/webgoat-2023-4-ethical-web-hacking/, however I was unable to complete the command "$ sudo apt-get install openjdk-17-jre", when I run it it replies that the package can not be found.
    - img src = Screenshot 2025-09-14 at 14.03.33.png
    - Therefore, I was unable to run the other commands either, since it did not work. 
# c) 
- Updated OS and applications on Linux by opening terminal and typing the commands: sudo apt-get update' and
'sudo apt-get dist-upgrade'.

# d) 
