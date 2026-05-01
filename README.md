# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>

## Output
```
Microsoft Windows [Version 10.0.26200.8246]
(c) Microsoft Corporation. All rights reserved.

C:\Users\acer>ping google.com

Pinging google.com [2404:6800:4007:833::200e] with 32 bytes of data:
Reply from 2404:6800:4007:833::200e: time=2ms
Reply from 2404:6800:4007:833::200e: time=8ms
Reply from 2404:6800:4007:833::200e: time=13ms
Reply from 2404:6800:4007:833::200e: time=11ms

Ping statistics for 2404:6800:4007:833::200e:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 2ms, Maximum = 13ms, Average = 8ms

C:\Users\acer>ipconfig

Windows IP Configuration


Wireless LAN adapter Local Area Connection* 1:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 2:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . :
   IPv6 Address. . . . . . . . . . . : 2406:7400:c4:d61d:dcd4:5ab:1a11:4c6e
   Temporary IPv6 Address. . . . . . : 2406:7400:c4:d61d:c433:77fa:eb70:ae77
   Link-local IPv6 Address . . . . . : fe80::cf03:77ac:9874:555b%11
   IPv4 Address. . . . . . . . . . . : 192.168.0.108
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : fe80::2a87:baff:fe00:fb69%11
                                       192.168.0.1

Ethernet adapter Ethernet:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

C:\Users\acer>tracert google.com

Tracing route to google.com [2404:6800:4007:833::200e]
over a maximum of 30 hops:

  1     1 ms     1 ms     2 ms  2406:7400:c4:d61d:2a87:baff:fe00:fb69
  2     5 ms     2 ms     2 ms  2406:7400:b0::16
  3     *        *        *     Request timed out.
  4     *        *        *     Request timed out.
  5     4 ms     2 ms     4 ms  2001:4860:1:1::1c38
  6     7 ms     2 ms     2 ms  2404:6800:8202:200::1
  7     9 ms     3 ms     3 ms  2001:4860:0:1::13de
  8     8 ms     2 ms     2 ms  2001:4860:0:1::5663
  9     2 ms     2 ms     2 ms  pnmaaa-an-in-x0e.1e100.net [2404:6800:4007:833::200e]

Trace complete.

C:\Users\acer>nslookup google.com
Server:  183.82.243.66.actcorp.in
Address:  183.82.243.66

Non-authoritative answer:
Name:    google.com
Addresses:  2404:6800:4007:83b::200e
          172.217.24.14


C:\Users\acer>netstat -an

Active Connections

  Proto  Local Address          Foreign Address        State
  TCP    0.0.0.0:80             0.0.0.0:0              LISTENING
  TCP    0.0.0.0:135            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:445            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:1309           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:3306           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:4343           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:4449           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:5040           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:5141           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:33060          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:46760          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49664          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49665          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49666          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49667          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49668          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49676          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:58995          0.0.0.0:0              LISTENING
  TCP    127.0.0.1:5141         127.0.0.1:55014        ESTABLISHED
  TCP    127.0.0.1:9993         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:11434        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:15152        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:19443        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46753        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46934        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46935        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46935        127.0.0.1:57546        ESTABLISHED
  TCP    127.0.0.1:46936        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46936        127.0.0.1:49685        ESTABLISHED
  TCP    127.0.0.1:46937        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46937        127.0.0.1:49688        ESTABLISHED
  TCP    127.0.0.1:49296        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:49669        127.0.0.1:49670        ESTABLISHED
  TCP    127.0.0.1:49670        127.0.0.1:49669        ESTABLISHED
  TCP    127.0.0.1:49671        127.0.0.1:49672        ESTABLISHED
  TCP    127.0.0.1:49672        127.0.0.1:49671        ESTABLISHED
  TCP    127.0.0.1:49673        127.0.0.1:49674        ESTABLISHED
  TCP    127.0.0.1:49674        127.0.0.1:49673        ESTABLISHED
  TCP    127.0.0.1:49679        127.0.0.1:49680        ESTABLISHED
  TCP    127.0.0.1:49680        127.0.0.1:49679        ESTABLISHED
  TCP    127.0.0.1:49681        127.0.0.1:49682        ESTABLISHED
  TCP    127.0.0.1:49682        127.0.0.1:49681        ESTABLISHED
  TCP    127.0.0.1:49683        127.0.0.1:49684        ESTABLISHED
  TCP    127.0.0.1:49684        127.0.0.1:49683        ESTABLISHED
  TCP    127.0.0.1:49685        127.0.0.1:46936        ESTABLISHED
  TCP    127.0.0.1:49686        127.0.0.1:49687        ESTABLISHED
  TCP    127.0.0.1:49687        127.0.0.1:49686        ESTABLISHED
  TCP    127.0.0.1:49688        127.0.0.1:46937        ESTABLISHED
  TCP    127.0.0.1:49689        127.0.0.1:49690        ESTABLISHED
  TCP    127.0.0.1:49690        127.0.0.1:49689        ESTABLISHED
  TCP    127.0.0.1:51779        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51780        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51781        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51782        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:54430        127.0.0.1:58995        ESTABLISHED
  TCP    127.0.0.1:55014        127.0.0.1:5141         ESTABLISHED
  TCP    127.0.0.1:57540        127.0.0.1:57541        ESTABLISHED
  TCP    127.0.0.1:57541        127.0.0.1:57540        ESTABLISHED
  TCP    127.0.0.1:57542        127.0.0.1:57543        ESTABLISHED
  TCP    127.0.0.1:57543        127.0.0.1:57542        ESTABLISHED
  TCP    127.0.0.1:57544        127.0.0.1:57545        ESTABLISHED
  TCP    127.0.0.1:57545        127.0.0.1:57544        ESTABLISHED
  TCP    127.0.0.1:57546        127.0.0.1:46935        ESTABLISHED
  TCP    127.0.0.1:58995        127.0.0.1:54430        ESTABLISHED
  TCP    127.0.0.1:58995        127.0.0.1:62643        ESTABLISHED
  TCP    127.0.0.1:58995        127.0.0.1:62658        ESTABLISHED
  TCP    127.0.0.1:62643        127.0.0.1:58995        ESTABLISHED
  TCP    127.0.0.1:62658        127.0.0.1:58995        ESTABLISHED
  TCP    192.168.0.108:139      0.0.0.0:0              LISTENING
  TCP    192.168.0.108:49418    4.213.25.242:443       ESTABLISHED
  TCP    192.168.0.108:50161    13.69.239.78:443       TIME_WAIT
  TCP    192.168.0.108:53534    202.83.24.145:80       TIME_WAIT
  TCP    192.168.0.108:53798    104.18.32.47:443       ESTABLISHED
  TCP    192.168.0.108:53800    4.213.25.240:443       ESTABLISHED
  TCP    192.168.0.108:53803    150.171.110.86:443     TIME_WAIT
  TCP    192.168.0.108:54448    204.79.197.222:443     ESTABLISHED
  TCP    192.168.0.108:58093    192.168.0.101:8009     TIME_WAIT
  TCP    192.168.0.108:58243    192.168.0.101:8009     ESTABLISHED
  TCP    192.168.0.108:64369    192.168.0.101:8009     ESTABLISHED
  TCP    192.168.0.108:65179    172.188.155.25:443     ESTABLISHED
  TCP    192.168.0.108:65275    20.42.73.28:443        ESTABLISHED
  TCP    [::]:80                [::]:0                 LISTENING
  TCP    [::]:135               [::]:0                 LISTENING
  TCP    [::]:445               [::]:0                 LISTENING
  TCP    [::]:3306              [::]:0                 LISTENING
  TCP    [::]:4343              [::]:0                 LISTENING
  TCP    [::]:4449              [::]:0                 LISTENING
  TCP    [::]:5141              [::]:0                 LISTENING
  TCP    [::]:33060             [::]:0                 LISTENING
  TCP    [::]:46760             [::]:0                 LISTENING
  TCP    [::]:49664             [::]:0                 LISTENING
  TCP    [::]:49665             [::]:0                 LISTENING
  TCP    [::]:49666             [::]:0                 LISTENING
  TCP    [::]:49667             [::]:0                 LISTENING
  TCP    [::]:49668             [::]:0                 LISTENING
  TCP    [::]:49676             [::]:0                 LISTENING
  TCP    [::]:58995             [::]:0                 LISTENING
  TCP    [::1]:15161            [::]:0                 LISTENING
  TCP    [::1]:15161            [::1]:53805            ESTABLISHED
  TCP    [::1]:15161            [::1]:53807            ESTABLISHED
  TCP    [::1]:15161            [::1]:63305            TIME_WAIT
  TCP    [::1]:15161            [::1]:63306            TIME_WAIT
  TCP    [::1]:42050            [::]:0                 LISTENING
  TCP    [::1]:53805            [::1]:15161            ESTABLISHED
  TCP    [::1]:53807            [::1]:15161            ESTABLISHED
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:50160  [2a06:98c1:3108::ac40:94eb]:443  ESTABLISHED
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:52091  [2603:1061:14:153::1]:443  CLOSE_WAIT
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:53374  [2603:1063:2000:1::254]:443  ESTABLISHED
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:54616  [2603:1030:b04:a::372]:443  ESTABLISHED
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:54905  [2404:6800:4003:c04::bc]:443  ESTABLISHED
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:55385  [2a03:2880:f335:120:face:b00c:0:167]:5222  ESTABLISHED
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:58491  [2603:1046:2000:60::83]:443  TIME_WAIT
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:58492  [2603:1046:c06:c72::2]:443  TIME_WAIT
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:58494  [2603:1046:c06:c53::2]:443  TIME_WAIT
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:60452  [2620:1ec:50::12]:443  ESTABLISHED
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:60823  [2600:140f:3:8a4::3114]:443  ESTABLISHED
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:61255  [2404:6800:4007:817::200e]:80  ESTABLISHED
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:62576  [2a03:2880:f335:120:face:b00c:0:167]:443  TIME_WAIT
  TCP    [2406:7400:c4:d61d:c433:77fa:eb70:ae77]:65209  [2620:1ec:50::12]:443  ESTABLISHED
  UDP    0.0.0.0:5050           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5355           *:*
  UDP    0.0.0.0:49665          *:*
  UDP    0.0.0.0:49992          104.86.188.56:443
  UDP    0.0.0.0:51734          104.18.32.47:443
  UDP    0.0.0.0:56234          23.15.138.149:443
  UDP    0.0.0.0:57893          *:*
  UDP    0.0.0.0:61288          *:*
  UDP    127.0.0.1:1900         *:*
  UDP    127.0.0.1:49664        127.0.0.1:49664
  UDP    127.0.0.1:53773        *:*
  UDP    127.0.0.1:57892        *:*
  UDP    192.168.0.108:137      *:*
  UDP    192.168.0.108:138      *:*
  UDP    192.168.0.108:1900     *:*
  UDP    192.168.0.108:53772    *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5355              *:*
  UDP    [::]:49665             *:*
  UDP    [::]:49992             [2600:140f:3::6856:bc38]:443
  UDP    [::]:51734             [2a06:98c1:3100::6812:202f]:443
  UDP    [::]:56234             [2600:140f:3::170f:8a95]:443
  UDP    [::]:61288             *:*
  UDP    [::1]:1900             *:*
  UDP    [::1]:53771            *:*
  UDP    [fe80::cf03:77ac:9874:555b%11]:1900  *:*
  UDP    [fe80::cf03:77ac:9874:555b%11]:53770  *:*

C:\Users\acer>arp -a

Interface: 192.168.0.108 --- 0xb
  Internet Address      Physical Address      Type
  192.168.0.1           28-87-ba-00-fb-69     dynamic
  192.168.0.101         54-f1-5f-d6-82-a9     dynamic
  192.168.0.110         5c-e9-31-b4-e5-ef     dynamic
  224.0.0.22            01-00-5e-00-00-16     static
  224.0.0.251           01-00-5e-00-00-fb     static
  224.0.0.252           01-00-5e-00-00-fc     static
  239.255.255.250       01-00-5e-7f-ff-fa     static
  255.255.255.255       ff-ff-ff-ff-ff-ff     static

C:\Users\acer>hostname
TMP215-75-G2

C:\Users\acer>getmac

Physical Address    Transport Name
=================== ==========================================================
FC-6D-77-99-F6-29   \Device\Tcpip_{6D7E9B31-CFF8-472E-A5CD-4962F5701FA1}
74-D4-DD-CF-7E-05   Media disconnected

C:\Users\acer>route print
===========================================================================
Interface List
  4...fc 6d 77 99 f6 2a ......Microsoft Wi-Fi Direct Virtual Adapter
 14...fe 6d 77 99 f6 29 ......Microsoft Wi-Fi Direct Virtual Adapter #2
 11...fc 6d 77 99 f6 29 ......Intel(R) Wi-Fi 6E AX211 160MHz
  9...74 d4 dd cf 7e 05 ......Realtek PCIe GbE Family Controller
  1...........................Software Loopback Interface 1
===========================================================================

IPv4 Route Table
===========================================================================
Active Routes:
Network Destination        Netmask          Gateway       Interface  Metric
          0.0.0.0          0.0.0.0      192.168.0.1    192.168.0.108     40
        127.0.0.0        255.0.0.0         On-link         127.0.0.1    331
        127.0.0.1  255.255.255.255         On-link         127.0.0.1    331
  127.255.255.255  255.255.255.255         On-link         127.0.0.1    331
      192.168.0.0    255.255.255.0         On-link     192.168.0.108    296
    192.168.0.108  255.255.255.255         On-link     192.168.0.108    296
    192.168.0.255  255.255.255.255         On-link     192.168.0.108    296
        224.0.0.0        240.0.0.0         On-link         127.0.0.1    331
        224.0.0.0        240.0.0.0         On-link     192.168.0.108    296
  255.255.255.255  255.255.255.255         On-link         127.0.0.1    331
  255.255.255.255  255.255.255.255         On-link     192.168.0.108    296
===========================================================================
Persistent Routes:
  None

IPv6 Route Table
===========================================================================
Active Routes:
 If Metric Network Destination      Gateway
 11   4136 ::/0                     fe80::2a87:baff:fe00:fb69
  1    331 ::1/128                  On-link
 11   4136 2406:7400:c4:d61d::/64   On-link
 11    296 2406:7400:c4:d61d:c433:77fa:eb70:ae77/128
                                    On-link
 11    296 2406:7400:c4:d61d:dcd4:5ab:1a11:4c6e/128
                                    On-link
 11    296 fe80::/64                On-link
 11    296 fe80::cf03:77ac:9874:555b/128
                                    On-link
  1    331 ff00::/8                 On-link
 11    296 ff00::/8                 On-link
===========================================================================
Persistent Routes:
  None

C:\Users\acer>netsh wlan show profiles

Profiles on interface Wi-Fi:

Group policy profiles (read only)
---------------------------------
    <None>

User profiles
-------------
    All User Profile     : EXAM-6
    All User Profile     : CODING TEST 1
    All User Profile     : AndroidAP_1418
    All User Profile     : SEC_LAB
    All User Profile     : ACTFIBERNET
    All User Profile     : OnePlus Nord CE4 Lite 5G
    All User Profile     : SHRUTHI
    All User Profile     : CODING TEST 2
    All User Profile     : CODING TEST 4
    All User Profile     : Galaxy A1377EE
    All User Profile     : CODING TEST 10
    All User Profile     : CODING TEST 3
    All User Profile     : vivo Y200 Pro 5G
    All User Profile     : SF
    All User Profile     : Jeeva
    All User Profile     : CODING TEST 5
    All User Profile     : CODING TEST 6
    All User Profile     : CODING TEST 7
    All User Profile     : SEC_WIFI
    All User Profile     : CPH1701
    All User Profile     : CODING TEST 11
    All User Profile     : CONNECT PANNIKO BROWW...♠️
    All User Profile     : ACTFIBERNET_5G
    All User Profile     : Basketball
    All User Profile     : 𝙼.𝙳𝚊𝚠𝚘𝚘𝚍
    All User Profile     : Nothing Phone (3a)_4594
    All User Profile     : Redmi 10 Prime
    All User Profile     : SEC_DRIVE
    All User Profile     : ASHWIN ROSHAN
    All User Profile     : OnePlus 11R 5G
    All User Profile     : CODING TEST 9
```
## Result
Thus Execution of Network commands Performed 
