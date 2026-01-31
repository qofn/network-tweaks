*(make sure your ethernet drivers are updated by going to your motherboards website and download the most recent audio drivers)*

- go to ethernet properties in controll panel - Control Panel > Network & Internet > Network & Sharing Center > Ethernet > Properties
turn of everything exept for IPV4 (if you live in a house with other people using wifi and have less then 500mbps download speed leave QOS Packet Scheduler ON)

----------------------------------------------------------

- download tpc optimzer - https://www.speedguide.net/downloads.php
start as admin

//GENERAL SETTINGS

max connection speed

check optimal at bottem hit apply changes dont restart, 

then check custom at the bottem change these settings: 

tcp window auto-tuning: normal

windows scaling: disabled

congestion control: CUBIC or NONE (try what works best for u)

RSS: disable

RSC: disable

ECN: disable

Checksum: disable

TCP Chimney: disable

LSO: disable

TCP 1323: disable

//ADVANCED SETTINGS

QOS NLA: optimal 1

Network Throttle: disable fffffff

System Resposiveness: gaming: 0

TCP ACK: disable

TCP No Delay: disable

TCP Del Ack: disable

Large System Cache: disable

NON Sack RTT: disable

//NOW RESTART YOUR COMPUTER

-------------------------------------

- Next go to Control Panel > Network & Internet > Network & Sharing Center > Ethernet > Properties > Configure

DISABLE ALL THESE SETTINGS BELOW

ARP OFFLOAD

FLOW CONTROL

INTERRUPT MODERATION

IPV4 CHECKSUM OFFLOAD

JUMBO FRAME

LARGE SEND OFFLOAD V2 IPV4 and IPV6

NS OFFLOAD

RECV SEGMENT COALESCING IPV4 and IPV6

SHUTDOWN WAKE ON LAN

TCP CHECKSUM OFFLOAD IPV4 and IPV6

UDP CHECKSUM OFFLOAD IPV4 and IPV6

WAKE ON MAGIC PACKET 

WAKE ON PATTERN MATCH

------------------------------------------

- NEXT RUN THE NETWORK TWEAKER.ps1 with powershell in admin

select your adapter from the top left

Disable all setting under POWER SAVING SETTINGS

and disable Network Direct and Task Offload in GLOBAL SETTINGS 

//THEN RESTART
