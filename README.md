# Exercise 1


![picture](images/ex01.png)

Three pairs of direct (point-to-point) connections are presented, each with unique subnets. 
- the connection between **PC2** and **PC3** is established using an **RJ-45** crossover cable
- **Crossover cable:** In contrast, a crossover cable has one end with the transmit and receive pairs reversed. It's used for direct connections between similar devices, such as connecting two computers or two switches/router without an intermediate device.
Let's examine the connection **PC2 => PC3**:

```
PC2:
IP address: 192.168.12.83
Subnet mask: 255.255.255.248
```

```
PC3:
IP address: 192.168.12.81
Subnet mask: 255.255.255.248
```


# Exercise 2

![picture](images/ex02.png)
Here are two network setups:

- **Switch** with 5 PCs <br>
- **Hub** with 5 PCs <br>

All IP addresses are configured statically within the same subnet (255.255.255.248).



Below is a comparison table of switches and hubs:
<table border="1">
  <tr>
    <th>Feature</th>
    <th>Switch</th>
    <th>Hub</th>
  </tr>
  <tr>
    <td>Functionality</td>
    <td>Operates at OSI Layer 2 (Data Link Layer)</td>
    <td>Operates at OSI Layer 1 (Physical Layer)</td>
  </tr>
  <tr>
    <td>Traffic Handling</td>
    <td>Uses MAC addresses to forward data only to the intended device</td>
    <td>Broadcasts data to all connected devices</td>
  </tr>
  <tr>
    <td>Performance</td>
    <td>Better performance in terms of speed and efficiency</td>
    <td>Slower performance due to shared bandwidth</td>
  </tr>
  <tr>
    <td>Cost</td>
    <td>Generally more expensive</td>
    <td>Relatively cheaper</td>
  </tr>
</table>





## What is OSI?

The **open systems interconnection (OSI)** model is a conceptual model created by the International Organization for Standardization which enables diverse communication systems to communicate using standard protocols. In plain English, the OSI provides a standard for different computer systems to be able to communicate with each other.
<br>
![picture](https://www.imperva.com/learn/wp-content/uploads/sites/13/2020/02/OSI-7-layers.jpg)


# Exercise 3

![picture](images/ex03.png)

I have configured a server rack containing four servers dedicated to different services:

- **HTTPS (Secure Hypertext Transfer Protocol):** Handles secure communication over the web.
- **FTP (File Transfer Protocol):** Manages file transfers between clients and servers.
- **DNS (Domain Name System):** Resolves domain names to IP addresses.
- **DHCP (Dynamic Host Configuration Protocol):** Automatically assigns IP addresses to devices on the network. <br>

###### These servers are interconnected through a switch. Additionally, there are six PCs connected to the same switch, obtaining their IP addresses dynamically from the DHCP server.

### Identify the port and OSI model layer for each protocol used:


- **HTTPS**: Port 443 (TCP), OSI Layer 7 (Application Layer)
- **FTP**: Port 20 (TCP) for data transfer, Port 21 (TCP) for control, OSI Layer 7 (Application Layer)
- **DNS**: Port 53 (TCP and UDP), OSI Layer 7 (Application Layer)

###  DNS Mapping


```
deep-in-net.local > 192.168.1.99
deep-in-net.com > deep-in-net.local
```

###### 192.168.1.99 is HTTPS Server IP

![picture](images/ex03a.png)
<br>
- **CNAME (Canonical Name):** Used in DNS to create aliases for domain names. Allows mapping multiple domain names to a single primary domain. Example: "www.example.com" can point to "example.com".
- **A Record (Address Record):** Fundamental DNS records mapping domain names to IP addresses. Converts human-readable domain names (like example.com) to numerical IP addresses (such as 192.168.1.1) used by computers on the Internet.

### Into Browser

![picture](https://01.kood.tech/git/root/public/media/branch/master/subjects/devops/deep-in-net/pictures/ex03-dns.jpg)


### Accessing to FTP server


![picture](https://01.kood.tech/git/root/public/media/branch/master/subjects/devops/deep-in-net/pictures/ex03-ftp.jpg)




# 



