# CECURE INTELLIGENCE COHORT4 INTERNSHIP

## Thursday Task Module1 Group4

* Code version control
* Branching & merging allow teammembers work concurrently
* Identity: Ensure differnt version of the doc are distinguished from each other
* Staging Area: Formatting and review of code.

 Source code management(SCM) to track modification to a souce code repository.



# Monday Task. 
## QUESTION 1: Describe any layered process you are familiar with similar to the OSI model

<b> APPLICATION LAYER:<b/> This is the seventh layer of the OSI model, The layer that humans interact with, examples of the application than human interface with are chrome, Firefox, skype, outlook etc. Application layer interface directly interacts with the application and provides common web application services. 
It depends on application protocols to function, they are embedded with the protocols that are needed to make the connection work HTTP, HTTPS. This layer takes the user input to produce the data to be transferred over the network. It allows user send data, access data and use networks The layer also facilitates communication and sometimes allow users to use software programs.
Application layer examples are: Telnet, File Transfer Protocol(FTP),Hypertext transfer protocol(HTTP).

### Functions of Application Layer
1.	It allows a user to access, retrieve and manage files in a remote computer.
2.	This layer provides services such as e-mail, file transfer, distributing results to users, directory services, network resources, and so on
3.	This layer allows users to interact with other software applications

### What are the NS IP addresses for Google, Facebook and Tesla Ip Address

GOOGLE Nameserver IP Address
IPv4: 8.8.8.8 and/or 8.8.4.4 .
IPv6: 2001:4860:4860::8888 and/or 2001:4860:4860::8844

Facebook Nameserver IP Address
IPV4: 157.240. 20.35.
IPv6: 2a03:2880:f11c:8183:face:b00c::25de

Tesla Nameserver IP Address
IPV4: 8.45.124.215
IPv6: 104.145.231.237

# Question 2. Breakdown the following RFC 1918 IPv4 address range into exactly 4 subnetwork with no address left over.”
#### 1. 10.10.10.0
#### 2. 192.168.0.0
#### 3. 172.168.1.0


---

## For 10.10.10.0

This is an IPv4 class A (range of 0-127)

To get the value of the subnet mask we can use a simple table

Subnet | 1 | 2 | 👉🏾 4 | 8 | 16 | 32 | 64 | 128 | 256 |
---| --- | --- | --- | --- | --- | --- | --- | --- | --- |
Host | 256 | 128 | 👉🏾 64 | 32 | 16 | 8 | 4 | 2 | 1 |
subnet mask | 8 | 9 | 👉🏾 10 | 11 | 12 | 13 | 14 | 15 | 16 |

so for 4 subnetwork the value is 10 i.e __10.10.10.0/10__
subnet mask = __255.192.0.0__ (in binary format)

And each subnetwork is within range of __64__

S/NO| Network ID | Broadcast ID | Useable IP Address
---| --- | --- | --- 
1 | 10.0.0.0/10 | 10.63.255.255/10 | 10.0.0.1/10 - 10.63.255.254/10
2 | 10.64.0.0/10 | 10.127.255.255/10 | 10.64.0.1/10 - 10.127.255.254/10
3 | 10.128.0.0/10 | 10.191.255.255/10 | 10.128.0.1/10 - 10.191.255.254/10
4 | 10.192.0.0/10 | 10.255.255.255/10 | 10.192.0.1/10 - 10.255.255.254/10

---

## For 192.168.0.0

This is an IPv4 class C (range of 192-223)

To get the value of the subnet mask we can use a simple table

Subnet | 1 | 2 | 👉🏾 4 | 8 | 16 | 32 | 64 | 128 | 256 |
---| --- | --- | --- | --- | --- | --- | --- | --- | --- |
Host | 256 | 128 | 👉🏾 64 | 32 | 16 | 8 | 4 | 2 | 1 |
subnet mask | 24 | 25 | 👉🏾 26 | 27 | 28 | 29 | 30 | 31 | 32 |

so for 4 subnetwork the value is 26 i.e __192.168.0.0/26__
subnet mask = __255.255.255.192__ (in binary format)

And each subnetwork is within range of __64__

S/NO| Network ID | Broadcast ID | Useable IP Address
---| --- | --- | --- 
1 | 192.168.0.0/10 | 192.168.0.63/10 | 192.168.0.1/10 - 192.168.0.62/10
2 | 192.168.0.64/10 | 192.168.0.127/10 | 192.168.0.65/10 - 192.168.0.126/10
3 | 192.168.0.128/10 | 192.168.0.191/10 | 192.168.0.129/10 - 192.168.0.190/10
4 | 192.168.0.192/10 | 192.168.0.255/10 | 192.168.0.193/10 - 192.168.0.254/10

---

## For 172.168.1.0

This is an IPv4 class B (range of 128-191)

To get the value of the subnet mask we can use a simple table

Subnet | 1 | 2 | 👉🏾 4 | 8 | 16 | 32 | 64 | 128 | 256 |
---| --- | --- | --- | --- | --- | --- | --- | --- | --- |
Host | 256 | 128 | 👉🏾 64 | 32 | 16 | 8 | 4 | 2 | 1 |
subnet mask | 16 | 17 | 👉🏾 18 | 19 | 20 | 21 | 22 | 23 | 24 |

so for 4 subnetwork the value is 18 i.e __172.168.1.0/18__
subnet mask = __255.255.192.0__ (in binary format)

And each subnetwork is within range of __64__

S/NO| Network ID | Broadcast ID | Useable IP Address
---| --- | --- | --- 
1 | 172.168.0.0/10 | 172.168.63.255/10 | 172.168.0.1/10 - 172.168.63.254/10
2 | 172.168.64.0/10 | 172.168.127.255/10 |  172.168.64.1/10 - 172.168.127.254/10
3 | 172.168.128.0/10 | 172.168.191.255/10 | 172.168.128.1/10 - 172.168.191.254/10
4 | 172.168.192.0/10 | 172.168.255.255/10 | 172.168.192.1/10 - 172.168.255.254/10






