## Set network parameters

### Tasks

0. Using any operating systems on which you can run the ``python`` interpreter and virtualbox software, map the network diagram below:

![alt text][network]

[network]: ./network.png "Logo Title Text 2"

1. Install and run the program on the 1 of computers  ``server.py`` available at ``https://github.com/jkanclerz/client-server-chat``
2. On 2 of the computers install and run the program ``client.py`` available at ``https://github.com/jkanclerz/client-server-chat``
3. By manipulating the network configuration at the virtualbox level, start the chat server, and make it available on the selected port and address so that other people within the class can connect to it (*It might not work as expected)
4. Install HTTP server software ``nginx`` or other, configure the index.html file according to the instructions, check the availability of the site using any ``HTTP`` protocol client from different IP configurations
5.  Use a program such as ``netstat`` or ``lsof`` to check the ports on which the chat or HTTP servers are running: ``netstat`` or ``lsof`` check on which ports the chat or HTTP servers are running

Initial network parameters
-------------------------
| Param | Value | comment |
| ------------- |:-------------:| -----:|
|   PC 1 |  
| IP - address  | 10.0.15.4 | |
| NETMASK  | /24 (255.255.255.0) | |
|   |  | |
| PC 2  |  | |
| IP - address  | 10.0.15.6 | |
| NETMASK  | /24 (255.255.255.0 )| |

Connection verification

Command
```
```

Effect
```
```

Static configuration of connection parameters
Initial network parameters
-------------------------
| Param | Value | comment |
| ------------- |:-------------:| -----:|
|   PC 1 |  
| IP - address  | 192.168.10.10 | |
| NETMASK  | 255.255.255.0 | |
|   |  | |
| PC 2  |  | |
| IP - address  | 192.168.10.11 | |
| NETMASK  | 255.255.128.0 | |
| PC 2  |  | |
| IP - address  | 172.16.100.100 | |
| NETMASK  | 255.255.0.0 | |

Connection verification

Command
```
```

Effect
```
```

New static configuration of connection parameters

-------------------------
| Param | Value | comment |
| ------------- |:-------------:| -----:|
|   PC 1 |  
| IP - address  |  | |
| NETMASKA  |  | |
|   |  | |
| PC 2  |  | |
| IP - address  |  | |
| NETMASKA  |  | |

Weryfikacja połączenia

Command
```
```

Effect
```
```

### Saving network configuration permanently

Why? how? what?

```
https://wiki.alpinelinux.org/wiki/Configure_Networking
```

### Good to know

-------------------------
| Param | Value | comment |
| ------------- |:-------------:| -----:|
| Location of the network configuration file| | |
| DOWN -> Disabling the network interface| | |
| UP -> Enabling interfejsu sieciowego| | |
| Checking the current parameters | | |
| listing of all interfaces | | |
| Which interfaces which ports are listening | | |

