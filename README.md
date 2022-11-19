# UGV_SKILL
Advanced_Networkin Advanced-Python

 ## Microtik Basic Configuration (LAN DHCP, WAN [DHCP Client/ Static IP / PPPOE Client]) 


#### 1. Selected Interface >> click YellowBox then Comment LAN And WAN
<img src="img/2022-11-18 (1).png">

#### 2. Click Ip Then Selected >> Addresses click Plus Icon Insert Private IP with Subnet Mask Like
`` 192.168.0.10/24 `` 
#### then Apply >> Ok



#### 3. Ip >> DHCP Client 

<img src="img/2022-11-18 (2).png">


#### 4. click Plus Icon  Select Interface WAN Then Apply And Ok
<img src="img/2022-11-18 (8).png">

#### 5. click IP >> DHCP Server
<img src="img/2022-11-18 (7).png">

<!-- <img src="img/2022-11-18 (9).png">


<img src="img/2022-11-18 (10).png"> -->


#### 6. Click DHCP Setup 
<img src="img/2022-11-18 (11).png">

#### 7. Then Next Next And OK
<img src="img/2022-11-18 (12).png">


#### 8. Then Setup SuccessFully
<img src="img/2022-11-18 (13).png">



### FireWall Rull
#### 10. IP >> select Firewall >> NAT
<img src="img/2022-11-18 (14).png">

#### 11. select Out Interface WAN 
<img src="img/2022-11-18 (15).png">

#### 12. Goto Action Option Then Select Masquerade
<img src="img/2022-11-18 (16).png">

## 2. Configure Microtik as a Router where WAN is using Static IP and LAN is using DHCP server.

#### 1.Goto Interfaces Then Comment WAN

<img src="img/day1.png">

#### 2. IP > Addreses click "+" Icon Then Assign Network Ip Address With Subnet Mask That Provide From ISP Select Interface (WAN) Then Click Ok
<img src="img/day2.png">

#### 3. Ip > Route Set DST. Adreses 0.0.0.0./0 Set The GateWay Provide From ISP It's Default   8.8.8.8 

<img src="img/day3.png">



