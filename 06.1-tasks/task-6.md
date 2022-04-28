# Dividing and aggregating the network

With the network address ``192.168.100.0/24``, divide the subnet with respect to the number of hosts

| subnet | number of hosts |
| ------------- |:-------------:|
| 1 | 64 |
| 2 | 16 |
| 3 | 4 |

-------------------------------

| Parameter | value | comment(opcional) |
| ------------- |:-------------:| -----:|
| The network address for the subdivision |  
| The network mask | |
| Binary net mask | |


2^(32 - mask length) - 2 >= required number of hosts

2^(32-26) - 2 = 62 too few
2^(32-25) - 2 = 126 >= OK

2^(32-28) -2 = 14 too few
2^(32-27) -2 = 30 >= 16 OK

| Subnet | Subnetwork address | Host min | Host max | Broadcast address |
| ------------- |:-------------: | -----: | -----: | -----: |
| 1 | 192.168.100.0/25 | 192.168.100.1 | 192.168.100.126 | 192.168.100.127 
| 2 | 192.168.100.128/27 | 192.168.100.129 | 192.168.100.158 | 192.168.100.159
| 3 | 