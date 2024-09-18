<u><h1>Establishing Azure Firewall on a Nginx Website</h1></u>
1.	Creating a Resource Group  “Network-RG” 
<br>
<a href="https://ibb.co/4mjKmJy"><img src="https://i.ibb.co/7YGjYbc/1.png" alt="1" border="0" /></a><br>

2.	Creating a Virtual Network VNet “New-Vnet”
<br>
<a href="https://ibb.co/2tXzYJ3"><img src="https://i.ibb.co/FwGQqp4/2.png" alt="2" border="0" /></a>
<br>
3.	Enabling Bastion to access the server for the configuration and installation of Nginx web server and also Firewall.
<br>
<a href="https://ibb.co/ZfjtTHC"><img src="https://i.ibb.co/HKS1gNQ/3.png" alt="3" border="0" /></a>
<br>
4.	Creating Virtual Machine “ngnix-web-VM” to host the Nginx server.
<br>
<a href="https://ibb.co/729HC2h"><img src="https://i.ibb.co/hDqk9D0/4.png" alt="4" border="0" /></a>
<br>
5.	Configuring Vnet for the VM.
<br>
<a href="https://ibb.co/R99yRn4"><img src="https://i.ibb.co/KXXwTZz/5.png" alt="5" border="0" /></a>
<br>
6.	Connecting to ngnix-web-VM server through Bastion connection.
<br>
<a href="https://ibb.co/rHsqkgR"><img src="https://i.ibb.co/zZJCs1T/6.png" alt="6" border="0" /></a>
<br>
7.	Login to the server.
<br>
<a href="https://ibb.co/QQLht5F"><img src="https://i.ibb.co/2hxRHb7/7.png" alt="7" border="0" /></a>
<br>
8.	Installing Nginx application on the Server.
<br>
<a href="https://ibb.co/SVRNsbH"><img src="https://i.ibb.co/Yfp2RmJ/8.png" alt="8" border="0" /></a>
<br>
9.	Creating index.html file at /var/www/html to create the website.
<br>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/fxxzdvD/10.png" alt="10" border="0" /></a>
<br>
10.	Creating content on the website.
<br>
<a href="https://ibb.co/nzqYKcR"><img src="https://i.ibb.co/RzGsJ07/9.png" alt="9" border="0" /></a>
<br>
11.	Restarting the Nginx application.
<br>
<a href="https://ibb.co/yXbcsgf"><img src="https://i.ibb.co/rm1Ry57/11.png" alt="11" border="0" /></a>
<br>
12.	Configuring Azure Firewall "New-Vnet-Firewall".
<br>
<a href="https://ibb.co/zNk8NDP"><img src="https://i.ibb.co/vDtsDRL/12.png" alt="12" border="0" /></a>
<br>
13.	In Azure Firewall configuring firewall policy.
<br>
<a href="https://ibb.co/VY3bmDv"><img src="https://i.ibb.co/KxmBw79/13.png" alt="13" border="0" /></a>
<br>
14.	Adding rule collection.
<br>
<a href="https://ibb.co/hFv7CRF"><img src="https://i.ibb.co/QvGbXFv/14.png" alt="14" border="0" /></a>
<br>
15.	Adding Destination Network Address translation (DNAT) rule.
<br>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/jyWJXD8/17.png" alt="17" border="0" /></a>
<br>
