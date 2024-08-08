<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Domain Pswd and Account Lockout Policies with Group Policy</h1>
This tutorial outlines the implementation of deploying domain pswds and account lockout policies with with group policy in Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Configure Domain Pswd and Account Lockout Policies with Group Policy](https://youtu.be/cG7M3Z-Cek4)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services

  

<h2>Operating Systems Used </h2>

- Windows Server 2022

<h2>High-Level Deployment and Configuration Steps</h2>

- Changing the password policies on Default Domain Policy
- Changing the account lockout policy
- Verifying changes by using command prompt
- Testing lockout policy



<h2>Deployment and Configuration Steps</h2>

<p>



</p>
<p>
Diagram
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/5fdd6f02-f36c-45fc-a0e0-ffcbeacdc797" height="80%" width="80%""/>
<img src="https://github.com/user-attachments/assets/d8a4070d-b07f-463c-bc86-986b0b1c0c49" height="80%" width="80%""/>
 <img src="https://github.com/user-attachments/assets/3bf06232-5416-4be2-ba4d-347cb9081c45" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/d110f6c6-49e2-483a-a7a7-d12ec39d8121" height="80%" width="80%""/>
   <img src="https://github.com/user-attachments/assets/f28a6d14-b61f-4767-9f65-c580a3b7127a" height="80%" width="80%""/>
</p>
<p>
In my Default Domain Policy, I was able to make Password Policy changes to enforcing password history, Min pswd age, min pswd length, and pswd meet complexity.
</p>
<br />


<p>
  <img src="https://github.com/user-attachments/assets/5f41e87f-c365-49d0-8ea1-a2fdc6097aae" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/468d9e6b-eaeb-4adc-a4ae-12b6ba40656f" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/0c273c6b-e177-4aef-bf7f-c5d42c4dff1a" height="80%" width="80%""/>
</p>
<p>On Account Lockout Policy, I was able to make changes to account lockout duration, account lockout threshold ,and reset account counter.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/53b9a0e1-7342-4181-a1bb-997de7f82f27" height="80%" width="80%""/>
</p>
<p>
Running gpupdate /force on command prompt to check update verification.
</p>

<p>
    <img src="https://github.com/user-attachments/assets/dd4edc4b-8b01-48b9-aba7-cea2f10bdae8" height="80%" width="80%""/>
</p>
<p>
  Testing the lockout policies on Jackie.Robbins account. 
</p>
<p>
    <img src="https://github.com/user-attachments/assets/25a81753-5d6e-4494-85ad-6d983e0ec720" height="80%" width="80%""/>
</p>
<p>
  Logged back into admin account and unlocked user Jackie Robbins' acount.
</p>
<br />
