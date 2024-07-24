# Steps for Windows Hardning

**A) Setting Hostname**

**1) Method 1: Using the GUI**

<span style="background-color: yellow;font-weight: bold;" >Open Server Manager:</span>

![](images/1.jpg){: style="height:600px;width:500px"}


<br><br>
<span style="background-color: yellow;font-weight: bold;" >Click on the ‘Local Server’ from the left sidebar menu and click on the ‘Computer name’.:</span>

![](images/2.jpg){: style="height:600px;width:750px;border:2px solid black;"}

<br><br>
<span style="background-color: yellow;font-weight: bold;" >The <b>‘System Properties’</b> dialog appears on the screen. Click on the <b>‘Change’</b> button in the ‘Computer Name’ tab.</span>

![](images/3.jpg){: style="height:600px;width:750px;border:2px solid black;"}

<br><br>
<span style="background-color: yellow;font-weight: bold;" >Enter the server name in the ‘Computer name’ field that you want to use as a server name.</span>

![](images/5.jpg){: style="height:500px;width:400px;border:2px solid black;"}


<span style="background-color: yellow;font-weight: bold;" >OK , SAVE , Restart Computer and its Done</span>
<hr style="border: 2px solid blue;">



<span style="background-color: yellow;font-weight: bold;" >Assign Ip Address to required interfaces </span></br>
`press WIN+R and type ncpa.cpl and hit ok`

![](images/ip1.jpg){: style="height:400px;width:600px;border:2px solid black;"}
<br><br>



<span style="background-color: yellow;font-weight: bold;" >identify interfaces to assign ip address, like below and double clik on it </span></br>

![](images/ip3.jpg){: style="height:500px;width:800px;border:2px solid black;"}

<br><br>
<span style="background-color: yellow;font-weight: bold;" >On double click you will  get below like dialog box ,click on Properties </span></br>

![](images/ip4.jpg){: style="height:500px;width:800px;border:2px solid black;"}


<br><br>
<span style="background-color: yellow;font-weight: bold;" > After click on Properties you will  get below like dialog box , now double click on internet protocol version 4</span></br>

![](images/ip5.jpg){: style="height:600px;width:500px;border:2px solid black;"}

<br><br>
<span style="background-color: yellow;font-weight: bold;" > select on red mark and insert your ip and click on save .</span></br>

![](images/ip6.jpg){: style="height:600px;width:500px;border:2px solid black;"}

<hr style="border: 2px solid blue;">

<br><br>
<span style="background-color: yellow;font-weight: bold;" > Check Partitions as per requirnment.</span></br>

![](images/partition.jpg){: style="height:100px;width:500px;border:2px solid black;"}

<hr style="border: 2px solid blue;">

<br><br>
<span style="background-color: yellow;font-weight: bold;" > Check for updates.</span></br>
go to the seach bar and type update and select check for updates.

![](images/a.jpg){: style="height:500px;width:600px;border:2px solid black;"}
<br><br>
<b>Clik on check fo rupdates , until you got below message , You are Update!!!<b><br>

![](images/b.jpg){: style="height:200px;width:600px;border:2px solid black;"}
<br>
<hr style="border: 2px solid blue;">
<br><br>
<span style="background-color: yellow;font-weight: bold;" > Power Setting</span></br>
<br>
Go to search bar and type Control Panel and clik on it.<br><br>
![](images/cp.jpg){: style="height:500px;width:600px;border:2px solid black;"}

<br>
Now Clik on category and select small icons.
<br>
![](images/cp2.jpg){: style="height:400px;width:750px;border:2px solid black;"}

<br>
Now Clik on Power Option.
<br>
![](images/cp3.jpg){: style="height:400px;width:1000px;border:2px solid black;"}

<br>
By default Balanced (recommonded) is selected. 
Click on Change plan setting.
<br>
![](images/cp4.jpg){: style="height:500px;width:700px;border:2px solid black;"}

<br>
A new windows will open , Set both setting as Never and click on Save changes.
<br>
![](images/cp5.jpg){: style="height:400px;width:600px;border:2px solid black;"}

<br>
Now Click on Change plan setting as shown below picture.<br>
![](images/cp6.jpg){: style="height:400px;width:800px;border:2px solid black;"}
<br>
A new windows will open , Set both setting as Never and click on Save changes.
<br>
![](images/cp5.jpg){: style="height:400px;width:600px;border:2px solid black;"}


<br>
Now click on arrow as show in picture 
<br>
![](images/cp7.jpg){: style="height:400px;width:700px;border:2px solid black;"}

<br>
Select change setting 
<br>
![](images/cp8.jpg){: style="height:400px;width:700px;border:2px solid black;"}


<br>
A new windows will open , Set both setting as Never and click on Save changes.
<br>
![](images/cp5.jpg){: style="height:400px;width:600px;border:2px solid black;"}


<br>
Select change setting 
<br>
![](images/cp9.jpg){: style="height:400px;width:700px;border:2px solid black;"}


<br>
A new windows will open , Set both setting as Never and click on Save changes.
<br>
![](images/cp5.jpg){: style="height:400px;width:600px;border:2px solid black;"}

<br>
<hr style="border: 2px solid blue;">
<span style="background-color: yellow;font-weight: bold;" > Disallow users from turning on/off windows firewall
</span></br><br>
Go to the run and type `gpedit.msc` and hit ok.<br>
![](images/gp1.jpg){: style="height:300px;width:600px;border:2px solid black;"}
<br><br>
 Nevigate to the `Computer Configuration --> Administrative Templates --> Network --> Network Connections --> Windows Firewall --> Standard Profile` 
 Refer below screenshot.
 <br>
 ![](images/gp2.jpg){: style="height:800px;width:1600px;border:2px solid black;"}<br>
 <br>
 Double click on `Windows Defender Firewall: Protect all network connections` it will open new windows like below.
 <br>Select `Enable ` button and then `Apply`then`Ok` <br>
![](images/gp3.jpg){: style="height:500px;width:600px;border:2px solid black;"}<br> 
<br>
<hr style="border: 2px solid blue;">
<br>
<span style="background-color: yellow;font-weight: bold;" > Digitally sign communications (always) <span>
<br>

Go to the run and type `gpedit.msc` and hit ok.

<br>
![](images/gp1.jpg){: style="height:300px;width:600px;border:2px solid black;"}<br>
<br>Nevigate to path `Computer Configuration\Windows Settings\Security Settings\Local Policies\Security Options`
Refer below screen
<br>
![](images/gp5.jpg){: style="height:800px;width:1200px;border:2px solid black;"}<br>
<br>
Double click on `Microsoft network server: Digitally sign communications (always)` By default its disabled , make it enable `Apply` then `OK.`<br>

![](images/gp6.jpg){: style="height:500px;width:400px;border:2px solid black;"}<br>
<hr style="border: 2px solid blue;">
<br>
<span style="background-color: yellow;font-weight: bold;" > Enable the virtualization based security  <span>
<br>

Go to the run and type `gpedit.msc` and hit ok.
<br>

![](images/gp1.jpg){: style="height:300px;width:600px;border:2px solid black;"}

<br>
Nevigate to path `Computer Configuration > Administrative Templates > System > Device Guard.`
Click on Device Guard and on right side you will see `Turn On virtualisation Based Security.`
By default its Not Configured. See below image.
<br>

![](images/vs1.jpg){: style="height:500px;width:950px;border:2px solid black;"}
<br>
<br>
Click on `Turn On virtualisation Based Security.` and  select `Enable` then `Apply` and `OK`
<br>
![](images/vs2.jpg){: style="height:700px;width:700px;border:2px solid black;"}

<br>
<hr style="border: 2px solid blue;">
<br>