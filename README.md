<p align="center">
<img <img width="3000" height="1887" alt="ServiceNow-Logo" src="https://github.com/user-attachments/assets/2f360ea2-80b9-40d7-a605-9fb0a1055e9f"
"/>
</p>

<h1>ServiceNow User Administration (Managing Users, Groups, and Roles)</h1>
This tutorial explains the process of creating a new user group, adding group members, and modifying the incident form so it shows a new field.<br />

<h2>Environments and Technologies Used</h2>

- ServiceNow Personal Developer Instance

<h2>Operating System Used </h2>

- Windows 11 Pro

<h2>OBJECTIVE: Create a new user group known as "Strawberry Support" and add members to it.</h2>

<p>
<img <img width="1836" height="858" alt="image" src="https://github.com/user-attachments/assets/cbfc278c-1cce-49a3-a7d7-9bd87bb725c9"
" />

</p>
<p>
From a fresh PDI instance, navigate to All>User Administration> Groups.
</p>
<br />

<p>
<img <img width="1889" height="864" alt="image" src="https://github.com/user-attachments/assets/7619ad89-e2e3-483e-9e27-8b0b55becb66"
" />

</p>
<p>
Open the Service Desk record. Select the Groups Tab. Select New to add a new group to Service Desk. 
</p>
<br />

<p>
<img <img width="1849" height="755" alt="image" src="https://github.com/user-attachments/assets/7b2f7f56-9994-4709-a403-7273344533eb"
 />


</p>
<p>
Populate the record as follows: 
  
-Name: Strawberry Support

-Manager: Fred Luddy

Select the Additional Options Menu, then select Save.
</p>
<br />

<p>
<img width="1324" height="817" alt="image" src="https://github.com/user-attachments/assets/4d4b0776-8fce-423a-9396-1f73ca4be5dd" />
  
</p>
<p>
Now that the account has been unlocked, go back to the client VM login and attempt to login with the correct password. Observe the success now that the account has been unlocked. 
</p>
<br />

<p>
<img width="492" height="545" alt="image" src="https://github.com/user-attachments/assets/74cc8c33-a8a7-4cfd-b2f6-8f0f6e1bf98f" />

</p>
<p>
Open the Domain Controller VM where AD Users and Computers should still be open, along with the find users window. Right click the client account and select "disable account". 
</p>
<br />

<p>
<img width="241" height="251" alt="image" src="https://github.com/user-attachments/assets/20543992-0053-4b98-8296-1c236713b023" />
  
</p>
<p>
Go to the client VM and logout then attempt to log back in. You will observe that the account is now disabled and login is not possible. 
</p>
<br />

<p>
<img width="509" height="538" alt="image" src="https://github.com/user-attachments/assets/df1f1b79-9df6-4a16-b679-a5541c8d2d1c" />

</p>
<p>
Go back to the Domain Controller VM and re-enable the account from the same window we had open previously. 
</p>
<br />

<p>
<img width="689" height="479" alt="image" src="https://github.com/user-attachments/assets/34677f2a-0c29-4ac4-8131-88d758265d4b" />

</p>
<p>
Proceed to the Client-side VM and attempt login. The system should let you in this time now that the account has been re-enabled. 
</p>
<br />
