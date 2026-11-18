# Networkwalks-B084-WK2-PM1-PM2-Brute-Force-Report

| **Pentester Name / (Cybersecurity Professional)** | Elijah Cauyan |
| --- | --- |
| **Batch** | B084-Networkwalks |
| **Date** | November 17, 2026 |
| **Modules Completed** | W3-PM1 / W3-P2M |
| **Target** | Locked PDF files |
| **Permission secured from client?** | Yes |
<br> 

<div align="center">

**LIABILITY DISCLAIMER**

</div>

During this report, I have performed brute-force attack activities on locked files, for which I was given authorization to break into. All the steps and procedures shown in the report are al purely for educational purposes and must not be used to harm others or break the law. The instructors, authors, and Networkwalks are not responsible for what you do with this knowledge, and any action you take is your own responsibility; misuse of knowledge can lead to criminal charges, penalties, and a permanent record.
<br> 
<br> 

<div align="center">
  
**INTRODUCTION**

</div>

In this report, I will showcase how I completed the tasks that I was given for my third-week internship at Networkwalks, which are WK3-PM1 and WK3-PM2, which focus on password cracking, also known as brute-force attacks.

Additionally, this report will cover how to install and use different brute-force attack tools such as locked PDF hash converter, John the Ripper, johnny, and Networkwalks tools. This set of tools is used to brute-force multiple locked PDFs, which I was given authorization to break into.
<br> 
<br> 

<div align="center">
  
**TOOLS USED**

</div>

| **Tool** | **Purpose** |
| --- | --- |
| Kali Linux OS | Operating System used for brute-force attack tools and activities. |
| Linux Terminal | Provides Linux command-line functionality. |
| John the Ripper | Identifies and tests password hashes to assess password strength |
| Johnny GUI | Provides a graphical interface for John the Ripper. |
| Online hashing tool (https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php) | Extracts password hashes from PDF files. |
| Networkwalks Hash Calculator | Networkwalks’ tool that calculates the hash digest of the files. |
| Networkwalks Password Cracker | Networkwalks’ tool that calculates the hash digest of the files. |

<br> 
<div align="center">

**ACTIVITIES PERFORMED**

</div>

**Johnny**

Figure 1: Install johnny
![](1install.png)
<br>
Figure 1.1: Run johnny
![](2launch.png)
<br>
Figure 1.2: Check John the Ripper directory
![](3checkJohnPath.png)
<br>
As shown in Figure 1, johnny was installed using the command “sudo apt install johnny” and not with the usual johnny install because there is no ready-to-go johnny for Linux, whereas for Windows, it is just an executable download and ready-to-go.

Additionally, as shown in Figure 1.1, johnny was opened by executing the command “johnny”. After opening johnny, I checked the directory of John the Ripper in johnny, because johnny will not work if it is not linked with John the Ripper’s executable, and to my surprise, johnny had already detected it, as John the Ripper comes pre-installed with Kali Linux, as shown in Figure 1.2

Figure 2: Find locked PDF’s hash digest
<br> 
![](4hash.png)
<br>
Figure 2.1: Create hash file
<br> 
![](5createHashFile.png) 
<br>
Figure 2.2: Paste hash digest
<br> 
![](6pasteHash.png) 
<br>
As shown in Figure 2, the locked PDF file was uploaded to the website “onlinehashcrack.com,” which provided the hash digest of the locked PDF. After obtaining the hash digest, I created a new file as shown in Figure 2.1 and pasted the hash digest as shown in Figure 2.2.

Figure 3: Open hash file in Johnny
![](7openHashFileInJohnny.png) 
<br>
Figure 3.1: Locate Hash File
<br> 
![](8locateHashFile.png) 
<br>
Figure 3.2: Start brute-force attack
![](9startBruteForce.png) 
<br>
Figure 3.3: Test password
![](10testPassword.png) 
<br>
Figure 3.4: Results
![](11complete.png) 
<br>
As shown in Figure 3, the hash file that was created in Figure 2.1 is being added in Johnny by opening File> Open Password File in the top-left corner. After, it redirected me to my thunar which I located the hash file as shown in Figure 3.1.

Additionally, once the setup was done with johnny and the hash file had been uploaded to John the Ripper, the next step I did was press “Start attack,” which showed me the password immediately, which is “good-luck”.

Furthermore, the password was tested as shown in Figure 3.3, which turned out to be correct, as shown in the results of Figure 3.4.

Lastly, repeat this step for the remaining PDFs as shown in the following Figures 4 – 4.2, and Figures 5 – 5.5.
<br> 
<br> 


**Repeat the process for the last 2 PDFs**

Figure 4: Find second locked PDF hash
![](12pdf2hash.png) 
<br>
Figure 4.1: Find third locked PDF hash
![](13pdf3hash.png) 
<br>
Figure 4.2: Paste each hash digest in their own files
<br> 
![](14hashFiles.png) 
<br>
Figure 5: Open the hash files in Johnny and start the attack
![](15hashFileInJohnny.png) 
<br>
Figure 5.1: After the attack
![](16postAttack.png) 
<br>
Figure 5.2: Test locked PDF 2 password
![](17testPassword2.png) 
<br>
Figure 5.3: Locked PDF 2 results
![](18.complete2.png) 
<br>
Figure 5.4: Test locked PDF 3 Password
![](19testPassword3.png) 
<br>
Figure 5.5: Locked PDF 3 results
![](20complete3.png)
<br>
**Networkwalks Tools**

Figure 6: Get locked PDF hash with Networkwalks’ hashing tool
![](21findHash.png) 
<br>
Figure 6.1: Paste hash
![](22pasteHash.png) 
<br>
Figure 6.2: Start cracking
![](23startCracking.png) 
<br>
Figure 6.3: Password Found
![](24passwordFound.png) 
<br>
Figure 6.4: Test Password
![](25testPassword.png) 
<br>
Figure 6.5: Results
![](26results.png) 
<br>
As shown in Figure 6, the locked PDF file was uploaded to Networkwalks’ hash calculator, which will be used later in the password cracking tool, similar to the Johnny task I had completed earlier in the report.

Additionally, after copying the hash digest, I pasted it into Networkwalks’ password cracking tool as shown in Figure 6.1. After pasting, I started cracking as shown in Figure 6.2.

Lastly, after the cracking process finished, the tool concluded the password as “password1” as shown in Figure 6.3. The password was then tested in the PDF, as shown in Figure 6.4, and it turned out to be the correct one, as shown in Figure 6.5.
<br> 
<br> 

<div align="center">

**CONCLUSION**

</div>

In conclusion, I have successfully completed the tasks I was given for my internship with Networkwalks, which are WK3-PM1 and WK3-PM2, which focus on brute-force attacks on locked PDFs. I was given authorization to do a brute-force attack on these files using various tools such as Johnny GUI, also known as John the Ripper in the backend, hashing, and Networkwalks’ brute-force attack tools. The password for each PDF is:

- Locked PDF1 Password: “good-luck”

- Locked PDF2 Password: “password1”

- Locked PDF3 Password: “1qaz2wsx”

- Locked PDF1 (NW) Password: “password1”

As a student in cybersecurity and intern for Networkwalks, it has given me a wider idea on how attackers think and move, especially with the tasks given to me for the past couple of weeks.

I would like to thank Networkwalks for giving me this opportunity to be an intern at their organization, and a huge thanks to Sir Waqas Karim for the guidance throughout the internship.
