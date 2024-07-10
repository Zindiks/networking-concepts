# Excecise 1


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


# Excercise 2

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





# What is OSI?

The **open systems interconnection (OSI)** model is a conceptual model created by the International Organization for Standardization which enables diverse communication systems to communicate using standard protocols. In plain English, the OSI provides a standard for different computer systems to be able to communicate with each other.
![picture](https://www.imperva.com/learn/wp-content/uploads/sites/13/2020/02/OSI-7-layers.jpg)