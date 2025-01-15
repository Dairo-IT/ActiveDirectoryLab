<h1>Active Directory Home Lab</h1>

 ### [YouTube Demonstration](https://youtu.be/oGYnP79Ccww?si=b3hSKf0DNXGkoxvA)

<h2>Description</h2>
In this lab, we're going to walk through how to create an Active Directory home lab environment using Oracle Virtual Box. Configuring and running this lab will definitely help develop your understanding of how Active Directory and Windows networking works. I'd highly recommend running through it a couple of times. Ask questions where stuff is unclear. Please let me know if you have any questions!
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Windows Server 2019</b>

<h2>Program walk-through:</h2>

<p align="center">
Visualization of what we are going to do: <br/>
<img src="https://i.imgur.com/imtdD1g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

1.	Download Virtualbox
  
2.	Windows iso and 2019 two seperate machine

3.	After everything is downloaded and installed we're going to create our first bm which is going to be our domain controller which is going to house AD,

4.	We're going to give this vm 2 network adapters; one is going to connect to the outside internet and the oner one is going to be used  to connected to the virtual box kind of private network that the clints is going to connect to

5.	After that we're going to install server 2019 and then ew're going to assing ip addressing for the internal network , our external network will automnatically get ip addressing from our home network, after we have ip addressing setup wer'e going to name the server 

6.	Install AD

7.	Then we're going to configure Nat and routing so the clietns on the private network acan reach the internet through the domain controller

8.	Then we're going to setup DHCP on the domain controller  so when we create or win 10 machine it can automatically get an ip address

9.	And last we do in our DC before we create our windows 10 client vm we're going to run a powershell script that will automatically create 1000 user in AD. i'll explain it too

10.	After this we're going to create another virtual machine and install windows 10 on it and that vm will be connected to the private virtual box network that we create, we're going to name it Client1 and we're going to join to our domain and then we're going to long 

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
