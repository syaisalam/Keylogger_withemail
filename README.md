<h1>Keylogger with email capability</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Keystroke logging, often denoted as keylogging or keyboard capturing, are a form of malicious software, or spyware, that enables unauthorized data collection by a perpetrator. Depending on the specific type of keylogger, it can illicitly acquire passwords, capture screenshots, log accessed web pages, covertly intercept and pilfer emails and instant messaging conversations, and even gather sensitive financial details (including credit card numbers, PIN codes, and bank account information). The operator of the logging program holds the ability to retrieve this amassed data, potentially transmitting it to third parties with criminal intent. In line with these concerns, this project delves into the creation of a basic keylogger utilizing Python, which can subsequently transmit the gathered data via email.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Python</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="left">
In this program, the library pynput is imported with the module; Key and Listener. These module is used to capture key events from users : <br/>
<img src="https://i.imgur.com/GV43W83.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
<br /> 
<br />
With the Listener function, the on_press and on_release parameters allows the capture of the press and release of keys from the user : <br/>
<img src="https://i.imgur.com/jfJ2q7D.png" height="30%" width="30%" alt="Disk Sanitization Steps"/>
<br /> 
<br />
The keys are collected in the form of arrays and converted to str. The count element triggers the function email after 10 counts: <br/>
<img src="https://i.imgur.com/vJc9wPO.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
<br />
<br />
This function will allow the message being collected to be more read-friendly before sending to email. The quotation marks, space keys and other keys presses (eg shift, ctrl, alt etc) other than digits are ensured to be recorded as space for readability purposes :  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
This function defines how the program will be closed; by pressing on the esc key : <br/>
<img src="https://i.imgur.com/1VfEoxp.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
<br /> 
<br />
In the send_email file, smtplib and ssl library are imported to allow server connections to the google account :  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The function will need a receiver and sender email to sending and receiving purposes. Note: the google account must be configured to allow control access to less secure apps <br/>
<img src="https://i.imgur.com/q04yMNH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
