<h1>Active Directory - Bulk User Creation</h1>

<h2>Description</h2>
In this lab I;ll walk you through how to create an Active Directory lab environment and quickly add 1,000 users with a Powershell script using Oracle Virtual Box. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Oracle Virtual Box</b>

<h2>Walk-through:</h2>

<p align="center">
Here is a diagram showing the full scope of the project<br/>
<img src="https://i.imgur.com/9APq5DD.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Set Up IP Address for Internal Network  <br/>
<img src="https://i.imgur.com/n3rbhie.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Set Up Our Domain Name <br/>
<img src="https://i.imgur.com/lPOIYh7.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Here is the text file for the names of 1,000 users that will be added to domain <br/>
<img src="https://i.imgur.com/1dSoonT.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Using Powershell, input the following script  <br/>
<img src="https://i.imgur.com/2Wbfv6V.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Line 6 gets the plain text password and creates and object for it  <br/>
<img src="https://i.imgur.com/B5FijcV.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
This loop allows for each username to follow the format: first initial + last name (ex.akhan) <br/>
<img src="https://i.imgur.com/58Y5XbN.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Run the script and watch how the users are quickly created<br/>
<img src="https://i.imgur.com/xUZlJc9.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Now from the Clients machine, we connect to the domain and restart our machine<br/>
<img src="https://i.imgur.com/r1NJqWM.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Check our domain controller to see if we can find the clients machine is connected to IP<br/>
<img src="https://i.imgur.com/iazMmpT.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Now that our client is connected to our domain, the newly created users can sign in!<br/>
<img src="https://i.imgur.com/9ZDjWhH.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
<br />
<br />
Login was successful!<br/>
<img src="https://i.imgur.com/EBfbq0w.jpg" height="80%" width="80%" alt="Active Directory Steps"/>
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
