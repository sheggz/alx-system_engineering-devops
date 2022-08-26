# 0x07. Networking basics #0

## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

* OSI Model
> What it is
> How many layers it has
> How it is organized
* What is a LAN
> Typical usage
> Typical geographical size
* What is a WAN
> Typical usage
> Typical geographical size
* What is the Internet
> What is an IP address
> What are the 2 types of IP address
> What is localhost
> What is a subnet
> Why IPv6 was created
* TCP/UDP
> What are the 2 mainly used data transfer protocols for IP (transfer level on the OSI schema)
> What is the main difference between TCP and UDP
> What is a port
> Memorize SSH, HTTP and HTTPS port numbers
> What tool/protocol is often used to check if a device is connected to a network

## Resources
[OSI model](https://youtu.be/sCYkeo466Qs)
[Different types of networks](https://www.lifewire.com/lans-wans-and-other-area-networks-817376)
[Internet](https://www.lifewire.com/lans-wans-and-other-area-networks-817376)
[MAC Address](https://whatismyipaddress.com/mac-address)
[What is an IP address](https://www.bleepingcomputer.com/tutorials/ip-addresses-explained/)
[Private and public address](https://www.iplocation.net/public-vs-private-ip-address)
[IPv4 vs IPv6](https://www.webopedia.com/insights/ipv6-ipv4-difference/)
[Localhost](Localhost)
[TCP and UDP](https://www.howtogeek.com/190014/htg-explains-what-is-the-difference-between-tcp-and-udp/)
[TCP/UDP ports List](https://en.wikipedia.org/wiki/List_of_TCP_and_UDP_port_numbers)
[What is ping /ICMP](https://en.wikipedia.org/wiki/Ping_%28networking_utility%29)
[Positional parameters](https://wiki.bash-hackers.org/scripting/posparams)
### man or help
* `netstat`
* `ping`

## TASKS
1. *0-OSI_model* - what is the OSI model?
2. *1-types_of_network* - Types of Networks
3. *2-MAC_and_IP_address* - what is a MAC & IP Address
4. *3-UDP_and_TCP* - Questions on TCP and UDP
5. *4-TCP_and_UDP_ports* - Write a Bash script that displays listening ports.
> That only shows listening sockets
> That shows the PID and name of the program to which each socket belongs
6. *5-is_the_host_on_the_network* - Write a Bash script that pings an IP address passed as an argument.
> Requirements:
> Accepts a string as an argument
> Displays Usage: 5-is_the_host_on_the_network {IP_ADDRESS} if no argument passed
> Ping the IP 5 times
```
Example:

sylvain@ubuntu$ ./5-is_the_host_on_the_network 8.8.8.8
PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data.
64 bytes from 8.8.8.8: icmp_seq=1 ttl=63 time=12.9 ms
64 bytes from 8.8.8.8: icmp_seq=2 ttl=63 time=13.6 ms
64 bytes from 8.8.8.8: icmp_seq=3 ttl=63 time=7.83 ms
64 bytes from 8.8.8.8: icmp_seq=4 ttl=63 time=11.3 ms
64 bytes from 8.8.8.8: icmp_seq=5 ttl=63 time=7.57 ms

--- 8.8.8.8 ping statistics ---
5 packets transmitted, 5 received, 0% packet loss, time 4006ms
rtt min/avg/max/mdev = 7.570/10.682/13.679/2.546 ms
sylvain@ubuntu$
sylvain@ubuntu$ ./5-is_the_host_on_the_network
Usage: 5-is_the_host_on_the_network {IP_ADDRESS}
sylvain@ubuntu$

```
---
## Author
Oluwasegun Ikoya

