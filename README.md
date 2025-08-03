<h1>Active Directory - Locked User Account Simulation</h1>



<h2>Description</h2>
This lab consists of creating a group policy in active directory of 3 login attempts before a user is logged out of their account for 30 minutes. I then ran a simulation of a user (my own Windows 11 Virtual Machine) locking themselves out of their account. I then reset the user's password allowing them access back into their account. Simulating a very common helpdesk/entry level IT situation.
<br />



<h2>Environments Used </h2>

- <b>Windows 11 VM
- Windows 2022 VM Server </b> 

<h2>Program walk-through:</h2>

<p align="center">
First, I created the group policy of allowing a user to attempt a login 3 times before their account becomes locked for 30 minutes: <br/>
<img src="https://i.imgur.com/FIwh3nz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Using a seperate windows 11 VM connected to my server, I incorrectly entered the password to lock them out of the account:  <br/>
<img src="https://i.imgur.com/oYHAfgy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Back on the server VM, I search the user's name and am able to reset their password: <br/>
<img src="https://i.imgur.com/906gaLR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Creating new password for user:  <br/>
<img src="https://i.imgur.com/flfZp9F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
User successfully logged in:  <br/>
<img src="https://i.imgur.com/DtAYILs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
