<h1>New HDD/SSD not showing in Windows10/11</h1>

<h2>Description</h2>
Project consists of a simple command prompt process to find what disks are recognized by the computer, which are showing and not showing in File Explorer, cleaning the one you just installed, formatting it for the computer to read, and assigning a letter to the drive for Windows to deisplay it in File Explorer.


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
Open Command, Type -DiskPart- and hit enter<br/>
<img width="1115" height="628" alt="image" src="https://github.com/user-attachments/assets/0f0ab992-08a7-43fe-a7f1-24ffa09abb40" />
<br />
<br />
type "list disk" and hit enter. You can see there are 3 disks on this computer but only 1 is in "this PC" <br/>
<img width="1283" height="989" alt="image" src="https://github.com/user-attachments/assets/2e916d65-9570-4b96-b570-51d994db92ef" />
<br />
<br />
Select the disk with "select disk _"<br/>
<img width="981" height="531" alt="image" src="https://github.com/user-attachments/assets/e3a92617-2300-4f12-bb05-73a8950c0448" />
<br />
<br />
Type "clean" to make sure nothing is on it anymore <br/>
<img width="986" height="522" alt="image" src="https://github.com/user-attachments/assets/5041db45-3a37-4aeb-b123-741d839aab23" />
<br />
<br />
Next type "create partition primary" this will get the drive ready to be formated<br/>
<img width="975" height="313" alt="image" src="https://github.com/user-attachments/assets/047e242c-47f7-42a2-9a93-2f8973ec27af" />
<br />
<br />
Now type "format fs=ntfs quick" so the computer can use it. NTFS is the default file system for Windows. (if there are errors using this method, run it again with "format fs-ntfs" this method (without "quick" at the end) scans the drive for errors but takes very long. In our case it formated just fine <br/>
<img width="747" height="244" alt="image" src="https://github.com/user-attachments/assets/32cd1c1c-29ce-462e-9ca3-13bef77f5dae" />
<br />
<br />
 Last we type "assign" and this will give the drive a letter to be displayed in File Explorer.<br/>
 <img width="1362" height="968" alt="image" src="https://github.com/user-attachments/assets/b8fd68d6-bbfa-458c-a7ed-38c16edc5fb6" />
<br />
<br />

With the last command sucessful, we can see it assigned the letter "E" to the new drive, and is now shown in File Explorer under "This PC".
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
