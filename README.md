<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Group Policy and Account Management</h1>
This walkthrough demonstrates how to configure Group Policy and provide System Administrative work within Active Directory.  <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)


<h2>Walkthrough Steps</h2>

<p>
</p>
<p>
Log into DC-1 and configure Group Policy to lockout the account after 5 attempts. Use the Google Drive below to learn how to configure the Account Lockout Threshold:
[How To Configure Account Lockout Threshold in Group Policy](https://docs.google.com/document/d/1msUMWaPDMR1hPYxzGOlgN4KpUjnyyYEv3vvOQXkSpLQ/edit)

<br />
<p>
<img src="https://github.com/user-attachments/assets/0b1a95ed-3a6d-4e68-84ed-d098e04be041" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>Next, pick a random user account you created previously and attempt to log in with it 6 times with a bad password.
<br />
<img src="https://github.com/user-attachments/assets/1a9f5e30-c5c9-4cd0-bbae-0e0acb22daea" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://github.com/user-attachments/assets/f501fba8-db6f-4e22-9ffb-75cae6b2d974" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://github.com/user-attachments/assets/36204be1-07ed-4413-bb45-ab9eab1ccc6a" height="60%" width="60%" alt="Disk Sanitization Steps"/>


</p>
<br />

<p> Now, go back to the Domain Controller (DC-1) and observe that the account has been locked out within Active Directory. Next, unlock the account and reset the password. 


<img src="https://github.com/user-attachments/assets/11f0e29e-f02c-415c-8aff-1d4de63caa25" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://github.com/user-attachments/assets/ffeaeb65-ef66-4cb9-be49-0b9085c082ed" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
You can also disable the same account within Active Directory.
</p>
<img src="https://github.com/user-attachments/assets/bfe55eb7-26a3-4a5f-bf59-cda52dc756c8" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
</p>
After you reset the password, attempt to log into Client-1 with the user account again. If you completed the steps correctly, you should be successfully logged into the user account. 
</p>
<img src="https://github.com/user-attachments/assets/021ffc7a-aaa9-436c-a5af-a32f5baf712e"
height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
</p>


