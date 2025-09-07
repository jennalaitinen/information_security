# Read and summarize: 

Karvinen 2021: Install Debian on Virtualbox
  - what is a virtualbx and how to download it
  - creating a new virtualbox and creating the account
  - how to install Debian on a Virtualbox

Karvinen 2020: Command Line Basics Revisited
  - the different commands used
  - important directories and how to use them
  - other useful commands

# a) Can't fish 
- I disabled the internet from the VM menu settings and also turned the "Enable network adapter" off.
- Made sure networking is off on my Linux - when attempting to change the ping a text pops up "Network is unreachable" meaning that my VM has currently no way to the outside network
- I tested the ping thing online aswell, and it worked - so i succesfully turned my VM offline.

# b) Local only
- When attempting to download the nmap, I noticed some error messages, I assumed they we're because my VM was offline, so I turned my VM off and changed the settings to online again, and managed to download the nmap.
- To safely do the port scanning, I shut down the VM again and turned off the network.
- I managed to do the port scanning. The nmap scanned 1 IP address and here are other things the nmap scanned:
    - Nmap scan report for localhost (127.0.0.1)
    - Other addresses for localhost (not scanned): ::1
    - Not shown: 999 closed tcp ports (reset)
    - Network distance: 0 hops
    - Nmap done: 1 IP address (1 host up) scanned in 8.22 seconds
    - Overall the experiment went well and I faced little trouble. I figured every problem by simply googling it or checking out course material.

  # c) Daemon scan
  - Succesfully installed Daemon
  - Information in terminal was quite similar with Deamon vs no Deamon containing some of the same information:
    - Other addresses for localhost (not scanned): ::1
    - Not shown: 998 closed tcp ports (reset) (one less than before)
    - Network distance: 0 hops
  - The information probably should've been significantly different than before but after using the commands and restarting a few times I still only got those results

  
