<h1>Active Directory Lab</h1>

 <h2>Description</h2>
    This project documents the setup and configuration of a Windows Server environment, including DHCP, Active Directory, RRAS, and user management tasks. The project uses PowerShell scripts and manual configurations to manage server roles, create users, and set up network services, with detailed steps captured in screenshots.
    <br />

 <h2>Languages and Utilities Used</h2>
    <ul>
        <li><b>PowerShell</b></li>
        <li><b>Active Directory Users and Computers</b></li>
        <li><b>DHCP Server Management</b></li>
    </ul>

 <h2>Environments Used</h2>
    <ul>
        <li><b>Windows Server 2022</b></li>
        <li><b>Windows 10</b> (21H2)</li>
    </ul>

<h2>Project walk-through:</h2>
<p style = "font-size: 40px;">
<b>Installing Windows Server 2022 in VirtualBox:</b> This step involves setting up a virtual machine in VirtualBox and installing Windows Server 2022 to serve as the foundation for the server environment. <br/>
<br />
<img src="https://i.imgur.com/Gp5alE1.png" height="80%" width="80%" alt="Installing Windows Server 2022"/>
<br />
<img src="https://i.imgur.com/6qjTJmM.png" height="80%" width="80%" alt="Windwos Server 2022 installed"/>
<br />
<br />
<b>Installing AD DS Role:</b> The Active Directory Domain Services (AD DS) role is installed to enable centralized management of users, computers, and other resources in the network.<br/><br />
<img src="https://i.imgur.com/Hvdyxth.png" height="80%" width="80%" alt="AD DS Installation"/>
<br />
<br />
<b>Promoting DC:</b> The server is promoted to a Domain Controller, establishing it as the primary server for managing the Active Directory domain. <br/><br />
<img src="https://i.imgur.com/9T6wZA6.png" height="80%" width="80%" alt="Promoting DC"/>
<br />
<br />
<b>Creating an OU and adding an admin user:</b> An Organizational Unit (OU) is created in Active Directory to organize objects, and an admin user is added for domain management.<br/><br />
<img src="https://i.imgur.com/MZ9gVC4.png" height="80%" width="80%" alt="Promoting DC"/>
<br />
<br />
<b>Giving Domain Admin access to the user:</b> The newly created user is granted Domain Admin privileges to allow full administrative control over the Active Directory domain.<br/><br />
<img src="https://i.imgur.com/uZR1URu.png" height="80%" width="80%" alt="Admin Access"/>
<br />
<br />
<b>Accessing DC with the newly created account:</b> The new admin account is used to log into the Domain Controller, verifying successful account creation and privilege assignment.<br/><br />
<img src="https://i.imgur.com/eufCVGe.png" height="80%" width="80%" alt="Accessing DC"/>
<br />
<br />
<b>Adding 10 new users into AD with PowerShell script:</b> A PowerShell script is executed to automate the creation of 10 new user accounts in Active Directory, streamlining user management.<br/><br />
<img src="https://i.imgur.com/GxHKGjp.png" height="80%" width="80%" alt="User Creation"/>
<br /> 
<br /> 
<img src="https://i.imgur.com/W1AcRgl.png" height="80%" width="80%" alt="User Creation"/>
<br />
<br />
<b>DHCP Server Configuration:</b> The DHCP server role is configured to dynamically assign IP addresses and network settings to devices on the network.<br/><br />
<img src="https://i.imgur.com/iNVJsmR.png" height="80%" width="80%" alt="DHCP Configuration"/>
<br />
<br />
<b>Creating New DHCP Scope:</b> A new DHCP scope is created to define a range of IP addresses that the DHCP server can assign to clients.<br/><br />
<img src="https://i.imgur.com/ggxmsak.png" height="80%" width="80%" alt="DHCP Scope"/>
<br />
<br />
<img src="https://i.imgur.com/mRe37q4.png" height="80%" width="80%" alt="DHCP Scope"/>
<br />
<br />
<b>Installing RRAS:</b> The Routing and Remote Access Service (RRAS) role is installed to enable routing and remote access capabilities on the server.<br/><br />
<img src="https://i.imgur.com/dJjMaG2.png" height="80%" width="80%" alt="DHCP Configuration"/>
<br />
<br />
<b>RAS NAT Configured:</b> Network Address Translation (NAT) is configured within RRAS to allow internal network devices to access external networks, such as the internet.<br/><br />
<img src="https://i.imgur.com/hd2suG4.png" height="80%" width="80%" alt="DHCP Configuration"/>
<br />
<br />
</p>
