
# VPC

## Tasks:

* Create a Virtual private cloud 
* Assign ip range of 10.0.0.0/16


<details>
           <summary>No of instances can be launched in VPC = 65536</summary>
           <p>Total No of machines in private cloud: 2^(32-x)</p>
           <p>Total no of machines available : 2^(32-x)-2(one ip for network and other for broadcast)</p>
           <p>Here we have x=16 </p>
           <p>hence total number of instances in private cloud is = 2^(32-16) = 65536 </p>
</details>

---
We have different types of servers
1. Web Server
2. Application Server
3. Database Server
---

We cannot dump all servers directly

1. Setting Webserver

web server = we want everyone in the world to access web server.
All incoming request will be sent to the web server. 
From webserver, request will be sent to Database server

2. Setting Database Server

User request, should not sent to Database directly (e.g. for banking application database is crucial part, we will keep it private for security purpose)

So, we will be creating two subnets

one subnet for webserver


one subnet for database server.


for one subnet, provide range 10.0.1.0/24

for second subnet, provide range 10.0.1.0/24


By default subnet are private.

we want to make one subnet as public.i.e. subnet which contains webserver

