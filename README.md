
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

