# Networking Commands
## 1. Ping
* Ping command is used to test the reachability and responsiveness of a host by sending ICMP (Internet Control Message Protocol)echo request packets and receiving echo reply packets in response.

- for example ``` ping google.com ```

## 2. Netstat  ( Network Statistics )
* Netstat displays active network connections on a system, including the protocol, local and foreign IP addresses, and the connection state.
- for example ``` netstat ```

- -a Displays all connections and listening ports (sockets), both TCP and UDP.
- -t	Shows only TCP connections.
- -u	Shows only UDP connections.
- -l	Displays only listening sockets (ports waiting for incoming connections).

## 3. ifconfig 
* ifconfig is used to display and configure network interface settings on a system.
- Network interfaces such as  (eth0, wlan0, lo, etc.)
- for example ``` ifconfig ```

## 4. Traceroute
* Traceroute command shows the path taken by packets and the transit time to reach a particular domain, IP address, or server.

- for example ``` traceroute youtube.com  ```

## 5. Tracepath
* Tracepath is used to identify the network path and delays to a destination host without requiring root privileges , simialr to traceroute.


- for example ``` tracepath youtube.com  ```

## 6. mtr   (my trace route)
* MTR is a network diagnostic tool that combines the functionality of ping and traceroute.

- for example ``` mtr google.com  ```

## 7. nslookup
* Nslookup is a DNS troubleshooting tool used to check domain-to-IP name resolution.

- for example ``` nslookup google.com  ```

## 8. Telnet
* Telnet is used to verify whether a domain or server is accessible on a specific port or not.

- for example ``` telnet google.com   80 ```

## 9. hostname 
* Hostname command is used to view or set the system’s name on a network.

- for example ``` hostname   ```

## 10 . IP
* IP command is used to show and configure IP addresses and network interfaces on a system.

- for example ``` ip address   show ```

## 11. iwconfig
* Iwconfig is used to display and configure information related to wireless network connections.

- for example ``` iwconfig   ```

## 12. ss
*  Netstat displays active network connections on a system, including the protocol, local and foreign IP addresses, and the connection state , similar to netstat.

- for example ``` ssa   ```

## 13 . dig 
* Dig is a DNS lookup tool used to obtain detailed DNS records and resolution information for a domain.

- for example ``` dns youtube.com   ```

## 14. whois
* Whois is used to retrieve domain registration information, such as where the domain is registered, ownership details, and registration dates.

- for example ``` whois  youtube.com   ```

## 15.  arp 
* ARP is used to map an IP address to its corresponding MAC address on a local network.

- for example ``` arp  ```

## 16.  ifplugstatus
* ifplugstatus is used to check whether a network interface is physically connected (plugged in) or not.

- for example ``` ifplugstatus  ```

# Daily use networking commands 

## 17. curl 
* Curl is a command-line tool used to interact with API endpoints and transfer data using protocols like HTTP and HTTPS.

* -X is used to define the HTTP request method (GET, POST, PUT, DELETE, etc.)

- for example ``` curl -X GET https://fake-json-api.mock.beeceptor.com/users  ```
* and to make it preety ues (jq)

- for example ``` curl -X GET https://fake-json-api.mock.beeceptor.com/users | jq  ```

## 18. Wget
* Wget is a command-line tool used to download files from the web.

- for example ``` Wget https://file-examples.com/wp-content/storage/2017/02/file_example_CSV_5000.csv ```

## 19. watch 
* watch is used to run a command repeatedly and display its output at regular intervals (by default every 2 seconds).


- for example ``` watch top   ```

## 20. nmap
* Nmap is used for network scanning to discover hosts, open ports, services, and security det

- for example ``` nmap -v google.com  ```

## 21. route
* Route command is used to view and manipulate the IP routing table of the system.

- for example ``` route  ```
