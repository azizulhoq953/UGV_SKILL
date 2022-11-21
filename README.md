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

#### 2. IP > Addreses click "+" Icon Then Assign Network Ip Address With Subnet Mask That
#### Provide From ISP Select Interface (WAN) Then Click Ok

<img src="img/day2.png">

#### 3. Ip > Route 

<img src="img/day3.png">

#### 4. Set DST. Adreses 0.0.0.0./0 Set The GateWay Provide From ISP It's Default   8.8.8.8 
<img src="img/day4.png">

## 3. Configure Microtik router as a Gateway where WAN haveing DHCP protocol, and configure lan network. 

#### 1. Go to Interface And Comment
#### 2. Go to IP >> Address Click On "+" Icon Then Write Private Ip With Subnet Mask Select the Interface (LAN) then OK

<img src="img/day3.1.png">

#### 3.Ip >> DHCP Client => click "+" and Select Interface (WAN) >> Apply And OK
<img src="img/day3.2.png">


#### 4. IP > DHCP Server => DHCP Setup => Select (LAN) Interface Now Click Next one by one
<img src="img/day3.3.png">

#### 5. IP > Firewall > NAT > Click "+" > Set 'Out Interface' As WAN > Goto Action Tab > Change Action to "masquerade" => Apply Then OK


## 4. Configure PPPOE Client on WAN interface, and implement local network (Using DHCP or PPPOE)


#### 1. Interfaces > Click "+" >PPPoE Client > Name The PPPoE >go to Dial Out > Now set User And Password > Make Sure That You Unmark "PaP" > Apply and Ok

<img src="img/day3.4.png">

#### 2.IP >Addreses > "+" > Assign Private Ip With Subnet Mask > Interface (LAN) > Apply Then Ok

<img src="img/day3.5.png">

#### 3. IP > DHCp Server > DHCP Setup > LAN Interface > Noew Click Next One by one

#### 4. IP > Firewal > NAT >Click "+" > Out Interface > As PPPOe Client Name > Action Tab >Change Action "Masquerade" > Apply Then Ok




