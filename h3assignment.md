# Read and summarize: 

Karvinen 2021: Install Debian on Virtualbox
  - what is a virtualbx and how to download it
  - creating a new virtualbox and creating the account
  - how to install Debian on a Virtualbox

Karvinen 2020: Command Line Basics Revisited
  - the different commands used for files, downloading and directories
  - important directories and how to use them
  - other useful commands

# a) Can't fish 
- I disabled the internet from the VM menu settings and also turned the "Enable network adapter" off. (Also disabled Wi-Fi from my whole computer)
- Made sure networking is off on my Linux - when attempting to change the ping (command: ping 8.8.8.8 - used to check network connectivity) a text pops up "Network is unreachable" meaning that my VM has currently no way to the outside network
- I tested the ping thing online aswell, and it worked - so i succesfully turned my VM offline. I turned VM offline every time I port scanned and when I needed to "sudo update" something I turned wi-fi on momentarily.
- By testing the ping I can tell if the network is disabled or not; if the message "Network is unreachable" pops up, this means that the adapter can't pick up the ping's address.
- If I got a reply along the lines of "ping 8.8.8.8 is ..." etc this means the internet is working at an IP level and can get access to the internet. 

# b) Local only
- When attempting to download the nmap, I noticed some error messages, I assumed they we're because my VM was offline, so I turned my VM off and changed the settings to online again, and managed to download the nmap.
- To safely do the port scanning, I shut down the VM again and turned off the network.
- I managed to do the port scanning. The nmap scanned 1 IP address and here are other things the nmap scanned directly from the terminal:
    - Nmap scan report for localhost (127.0.0.1) 127.0.0.1 is an internal address which is directed for my local computer and doesn't go out to the internet. 
    - Other addresses for localhost (not scanned): ::1
    - Not shown: 999 closed tcp ports (reset) The system has 1000 tcp ports in total, 999 ports closed means that the nmap "tried" 999 ports and the reply from them was that no
one is listening. Listening in this context means that your computer is waiting for connections. 
    - Network distance: 0 hops. 0 Hops means that the nmap reported that no packets left my computer (since I was not connected to the internet). 
    - Nmap done: 1 IP address (1 host up) scanned in 8.22 seconds
    - Overall the experiment went well and I faced little trouble. I figured every problem by simply googling it or checking out course material for advice or commands.

  # c) Daemon scan
  - Succesfully installed Daemon
  - Information in terminal was quite similar with Deamon vs no Deamon containing some of the same information:
    - Other addresses for localhost (not scanned): ::1
    - Not shown: 998 closed tcp ports (reset) (one less than before)
    - Network distance: 0 hops
  - The information probably should've been significantly different than before but after using the commands and restarting a few times I still only got those results

  # d) Bandit Oh-five
  - Managed to solve a few of the levels from Over The Wire:Bandit
  - I used the manual a bit for the start, since I was a bit confused but overall I think I progressed and managed to do the levels pretty good. I followed instructions and the commands needed.
  - I did levels 0-4

  # References:
  https://terokarvinen.com/information-security/
  
  https://terokarvinen.com/2021/install-debian-on-virtualbox/
  
  https://terokarvinen.com/2020/command-line-basics-revisited/
  
  https://nmap.org
  
  https://nmap.org/book/man-port-scanning-techniques.html
