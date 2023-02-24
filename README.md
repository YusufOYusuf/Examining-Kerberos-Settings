<h1>Examining Kerberos Settings</h1>


<h2>Description</h2>
In this lab, I examined Kerberos settings. Kerberos provides network security via SSO: nodes negotiate with each other on the word of a central Kerberos server operating as a trusted third-party. Users authenticate when they first connect. After that, the Kerberos protocol negotiates secure communications with other nodes, without further user input.
<br />



<h2>Environments Used </h2>

- <b>Windows Server 2016 Datacenter</b> 

<h2>Utilities and Language </h2>

- <b>Server Manager</b>

<h2>Program walk-through:</h2>

<p align="center">
Click on the start menu and navigate to Server Manager<br/>
<img src="https://i.postimg.cc/d1yD0cXw/Screen-Shot-2023-02-23-at-3-40-21-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
  
<br />
In the Server Manager window navigate to tolls and then click on group policy management<br>
<img src="https://i.postimg.cc/pLmBBp5Z/Screen-Shot-2023-02-23-at-3-42-26-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />



<br />
Now in the right pane click on forest > domains > ucertify.livelabs <br>
<img src="https://i.postimg.cc/d1JFdMN8/Screen-Shot-2023-02-23-at-3-45-44-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />



<br />
In the right pane click Linked group policy objects then right click default domain policy and click edit<br>
<img src="https://i.postimg.cc/sxZTgxPK/Screen-Shot-2023-02-23-at-3-48-31-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
In the left pane click Computer Configuration > Policies > Windows Settings > Security Settings > Account Policies > Kerberos Policy > Maximum Lifetime for Service Ticket<br>
<img src="https://i.postimg.cc/nzdvfJ62/Screen-Shot-2023-02-23-at-3-52-11-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
 
  
  
  
<br />
Change the maximum lifetime for service ticket properties <br>
<br> making this shorter could potentially increase security but could increase the load on a busy domain controller<br>
<img src="https://i.postimg.cc/cL487H6J/Screen-Shot-2023-02-23-at-3-56-45-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />  
  
  
  
  
  
  
  
  
  
