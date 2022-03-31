## Addressing in networks

![osi-iso](osi.svg)

## IP address structure

```192.168.100.192```
```255.255.255.0```




### How to count?
#### Network address

1. 
2.
3.

#### Broadcast address

1. 
2.
3.


## Dividing into an equal number of subnets

```2^S >= n```

Destination networks count 7 -> 2^3 >= 7
S -> how many bits needs to be traded in order to divide network into expected amount

Netmask -> 255.255.255.11100000 -> 255.255.255.224 -> /27


## Introduction

| decimal |  binary   | 
| ----------- | -----------  |
| ``10``  | | 
| ``92``  | | 
| ``37``  | | 
| ``240`` | | 
| ``192`` | | 
| ``255`` | | 
| ``128`` | | 
| ``168`` | | 

## 

| binary |  decimal   | 
| ----------- | -----------  |
| ``00100000``  |  | 
| ``11111000``  | | 
| ``10100000``  | | 
| ``00110000`` | | 
| ``10101100`` | | 
| ``01000000`` | | 
| ``11111100`` | | 
| ``01100010`` | | 
 
## CIDR notation
##  
| mask |  /(X) x - bits count   | 
| ----------- | -----------  |
| ``255.255.255.0``   | | 
| ``255.128.0.0``     | | 
| ``255.255.252.0``   | | 
| ``255.255.254.0``   | | 
| ``255.255.255.240`` | | 
| ``255.240.0.0``     | | 
## 

| CIDR |  mask   | 
| ----------- | -----------  |
| ``/8``    | | 
| ``/20``   | | 
| ``/30``   | | 
| ``/16``   | | 
| ``/27``   | | 
| ``/11``   | | 


## Number of hosts
## 
| sieć |  liczba   | 
| ----------- | -----------  |
| ``10.0.0.0/8``    | | 
| ``172.16.0.0/16``   | | 
| ``192.168.1.0/24``   | | 
| ``192.168.1.0/27``   | | 
| ``192.168.1.0/29``   | | 
| ``192.168.1.0/31``   | | 

* The number 0 in the mask?

## Parameters based on address

Given a host address and mask, find::
  * network address
  * initial host address in the network
  * number of hosts in a given subnet ```2^(32 bits - (net mask bits count)) - 2 (network and broadcast)```
  * the final host address range in the network
  * broadcast address



| Parameter |  value   | 
| ----------- | -----------  |
| ``ip``    | 192.168.1.145| 
| ``mask``   | 255.255.255.128 | 
| ``network address``   | |
| ``number of hosts``   | |
| ``host - min``   | | 
| ``host - max``   | | 
| ``broadcast``   | | 
 
## Assignment

0. Find all network parameters for a host with address 172.16.128.64 / 16
##   
| Parameter |  value   | 
| ----------- | -----------  |
| ``ip``    | 192.168.1.145| 
| ``maska``   | 255.255.255.128 | 
| ``network address``   | |
| ``number of hosts``   | |
| ``host - min``   | | 
| ``host - max``   | | 
| ``broadcast``   | | 

1.
  * Divide the network ```192.168.1.0/16``` into 16 equal subnets
##   
| Adres sieci |  zakres hostów   | Adres Rozgłoszeniowy |
| ----------- | -----------  | ----------- |
| ``192.168.1.0``    | | |
| ````   | | |
| ````   | | |
| ````   | | |
| ````   | | |
| ````   | | |

2. 
  * Divide the network ``172.16.0.0/16`` into 6 equal subnets.

3. 
  * Divide the network ``192.168.1.0/24``, so that each subnet has capacity of 11 hosts.

4. 
  * Divide the network ``10.0.0.0/8`` na 5 podsieci. 
    * Subnetwork A is to have 100,000 hosts,
    * B – 10 000 hosts
    * C – 3 000 hosts
    * D – 500 hosts
    * E – 2 hosts.
    
## Wizualizacja

![krakow siec akademicka](cracow-core.jpeg)


## Materiały

    * http://www.cyfronet.krakow.pl/sieci/13152,artykul,charakterystyka_sieci.html
    * https://www.computerworld.pl/news/Sieci-szkieletowe-polskich-operatorow,394360.html
    * https://cidr.xyz/

    * List of Polish address pools
    * http://42.pl/pl/networks.html?html=1