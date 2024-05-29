<h1>Observing RDP Brute Force with Azure Sentinel</h1>

<h2>Description</h2>
Project consists of using a custom PowerShell script to extract metadata from Windows Event Viewer that is forwarded to a third party API in order to derive geolocation data. We can configure Log Analytics Workspace in Azure to intake custom logs and construct custom fields by using a tailored code to map the geo data. By configuring Azure Sentinel, Microsoft's Cloud SIEM, it becomes possible to exhibit international attack data, RDP brute force, on a world map according to the physical location and magnitude of attacks. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Azure Sentinel</b>

<h2>Environments Used </h2>

- <b>Windows 11</b> (21H2)

<h2>Project walk-through:</h2>

<p align="center">
Setting Up VM: <br/>
<img src="https://i.imgur.com/HnCoEIR.png"/>
<br />
<br />
Use custom PowerShell script inside the VM to extract metadata:  <br/>
<img src="https://i.imgur.com/uXF2YEh.png"/>
<br />
<br />
Utilize custom code to make a custom log with the geodata from the failed RDP log file: <br/>
<img src="https://i.imgur.com/FCPcDyj.png"/>
<br />
<br />
Create map in workbooks with custom query to display the failed RDP brute force attacks:  <br/>
<img src="https://i.imgur.com/Bm383Mq.png"/>
<br />
<br />
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
