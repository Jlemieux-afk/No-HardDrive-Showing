<h1>New HDD/SSD not showing in Windows10/11</h1>

<h2>Description</h2>
Project consists of a simple command prompt process to find what disks are recognized by the computer, Cleaning the one you just installed, formatting it for the computer to read, and assigning a letter to the drive for Windows to deisplay it.


<h2>Languages and Utilities Used</h2>

- <b>Command</b> 
- <b>Diskpart</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
This PC shows the OS drive but not the other drives on the computer. <br/>
<img width="1310" height="762" alt="image" src="https://github.com/user-attachments/assets/6d0c3ebe-ecd8-443b-a4e5-fac3b066c484" />
<br />
<br />
Open Command, Type DiskPart and hit enter<br/>
<img width="1115" height="628" alt="image" src="https://github.com/user-attachments/assets/0f0ab992-08a7-43fe-a7f1-24ffa09abb40" />
<br />
<br />
type: list disk and hit enter. You can see there are 3 disks on this computer but only 1 is in "this PC" <br/>
<img width="1283" height="989" alt="image" src="https://github.com/user-attachments/assets/2e916d65-9570-4b96-b570-51d994db92ef" />

<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
