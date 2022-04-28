# Dividing and aggregating networks

With the network address ``192.168.1.0/24``, divide it into 4 equal subnets


| Parameter | value | comment(opcional) |
| ------------- |:-------------:| -----:|
| The address of the network to be subdivided |  
| The network mask | |
| Binary mask |

---------------------------

New subnet mask

```
2^n >= L
n - the number of ones to be added to the old mask address
L - the number of subnets into which the network is divided
```

2^n >= 4
2^2 >= 4

so n = 2

We have to give up 2 ones from the mask to the addresses of separated networks


| Subnet | Subnet address | Host min | Host max | Broadcast address |
| ------------- |:-------------: | -----: | -----: | -----: |
| 1 | 192.168.1.0 | 192.168.1.1 | 192.168.1.62 | 192.168.1.63 |
| 2 | 192.168.1.64 | 192.168.1.65 | 192.168.1.126 | |
| 3 | 192.168.1.128 | 192.168.1.129
| 4 |
