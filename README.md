# NETWORKWALKS-B083-WK3-PM1-PASSWORD-CRACKING-with-Network-walk-tools
**Password Cracking Using Network Walks Tools and John the Ripper**
**Project Overview**

This project was completed as part of the Network Walks B082 Cybersecurity Training Program.

The objective of this project is to understand the basic process of password cracking and password recovery using Network Walks tools and John the Ripper.

The project is divided into two modules.

##**Module 1 — John the Ripper Password Cracking**

This module covers:

Downloading John the Ripper
Installing and setting up John the Ripper
Working with the John the Ripper binaries
Using the Network Walks PDF Hash Cracker
Uploading a password-protected PDF
Extracting the generated hash
Creating a hash.txt file
Using the John the Ripper executable
Loading the hash file
Selecting the password file
Starting the password cracking process
Verifying the recovered password

##**Module 2 — Network Walks Hash Calculator and Password Cracker***

This module covers:

Using the Network Walks Hash Calculator
Uploading the authorized PDF
Generating/extracting the required hash
Using the Network Walks Password Cracker
Providing the hash to the password cracker
Recovering the password
Using the recovered password to open the authorized PDF files
Testing the recovered password with PDF 1, PDF 2, and PDF 3

Note: All activities documented in this repository were performed using authorized Network Walks lab files.

##**MODULE 1 — JOHN THE RIPPER PASSWORD CRACKING**
**Objective**

The objective of Module 1 is to understand how a password-protected file can be converted into a hash representation and then processed using John the Ripper for password recovery.

The overall workflow is:

Download John the Ripper
        ↓
Install / Extract John
        ↓
Locate John Binaries
        ↓
Open Network Walks PDF Hash Cracker
        ↓
Upload Locked PDF
        ↓
Generate / Copy Hash
        ↓
Create hash.txt
        ↓
Open John.exe
        ↓
Load hash.txt
        ↓
Select Password File
        ↓
Start Attack
        ↓
Password Cracked

**1. Download John the Ripper**

The first step was to download John the Ripper.

John the Ripper is an open-source password security auditing and password recovery tool. The official project provides binary distributions for supported platforms, including Windows.

**Steps**

Open the official John the Ripper website.
Navigate to the download section.
Download the required John the Ripper package for the system.
Save the downloaded file.
Extract the downloaded archive.

The official documentation explains that when a binary distribution is used, compilation is not required and John can be run from the extracted run directory.

**2. Install and Set Up John the Ripper**

After downloading John the Ripper, the archive was extracted.

The extracted directory contains the files and binaries required to run John the Ripper.

For example:

john/
│
├── run/
│
├── doc/
│
├── src/
│
└── other files


According to the official installation documentation, users of binary distributions can start John directly after extraction rather than performing a separate system-wide installation.

**3. Locate the John the Ripper Binaries**

Inside the extracted John the Ripper directory, the required executable and supporting files were located.

On Windows, the executable is generally:

john.exe

The exact executable and supporting files can vary depending on the John distribution. The official documentation notes that binary distributions may include alternate executables.

The run directory was therefore used as the main working directory.

**4. Open the Network Walks PDF Hash Cracker**

After setting up John the Ripper, the next step was to obtain the hash from the password-protected PDF.

The Network Walks PDF Hash Cracker was opened for this purpose.

The tool was used to process the authorized locked PDF and generate the corresponding hash information.

**5. Upload the Locked PDF**

The password-protected PDF provided for the Network Walks exercise was uploaded to the PDF Hash Cracker.

**Steps**

Open the PDF Hash Cracker.
Select the upload option.
Select the authorized locked PDF.
Upload the file.
Wait for the tool to process the file.

The tool then generated the hash information required for the next step.

**6. Copy the Generated Hash**

After uploading the PDF, the PDF Hash Cracker generated a hash.

The generated hash was copied from the tool.

The hash was then prepared for use with John the Ripper.


**7. Create hash.txt Using Notepad**

After copying the hash, Notepad was opened.

A new text file was created.

The copied hash was pasted into the file.

The file was saved as:

hash.txt

The final file structure was:

hash.txt

The file contained the generated lab hash.

**8. Open john.exe**

The John the Ripper run directory was opened.

The Windows executable was located:

john.exe

John the Ripper is intended to be run from a command-line shell rather than by simply double-clicking the executable. The official FAQ specifically notes this for Windows.

The command prompt was therefore opened in the John the Ripper run directory.

**9. Load the hash.txt File**

The hash.txt file created earlier was placed where John could access it, or its full path was supplied.

John was then started with the hash file:

john.exe hash.txt

John the Ripper accepts password/hash files as command-line arguments.


**10. Open the Password File**

For the password cracking process, the required hash file for the Network Walks exercise was selected.

**11. Start the Password Cracking Attack**

After loading the hash and selecting the required password file, the cracking process was started.

John then tested password candidates against the supplied hash.

The cracking process may take different amounts of time depending on the password, hash type, wordlist, and system.

**12. Display the Recovered Password**

After the password was recovered, the result was displayed

The recovered password was then recorded as part of the lab result.

##**MODULE 1 — RESULT**

The first module successfully demonstrated the complete password recovery workflow:

Locked PDF
    ↓
Network Walks PDF Hash Cracker
    ↓
Hash Generated
    ↓
Hash Copied
    ↓
hash.txt Created
    ↓
John the Ripper
    ↓
Password File / Wordlist
    ↓
Password Cracking
    ↓
Recovered Password

**MODULE 2 — NETWORK WALKS HASH CALCULATOR AND PASSWORD CRACKER**

**Objective**

The objective of Module 2 is to use the Network Walks Hash Calculator and Network Walks Password Cracker to work with the authorized PDF files and recover the required passwords.

The recovered password was then tested against the provided PDF files.

The workflow is:

Upload PDF
      ↓
Network Walks Hash Calculator
      ↓
Generate / Obtain Hash
      ↓
Copy Hash
      ↓
Network Walks Password Cracker
      ↓
Paste Hash
      ↓
Start Cracking
      ↓
Password Recovered
      ↓
Use Password on PDF 1
      ↓
Use Password on PDF 2
      ↓
Use Password on PDF 3

**1. Open Network Walks Hash Calculator**

The Network Walks Hash Calculator was opened.

This tool was used to process the authorized PDF provided for the exercise and obtain the required hash information.

**2. Upload the PDF**

The authorized PDF file was uploaded to the Network Walks Hash Calculator.

**Steps**

Open the Hash Calculator.
Select the upload option.
Choose the PDF provided for the Network Walks exercise.
Upload the file.
Wait for the tool to process the file.

**3. Generate / Obtain the Hash**

After the PDF was uploaded, the Hash Calculator generated the required hash.

The generated hash was copied for use in the next step.

**4. Open Network Walks Password Cracker**

The Network Walks Password Cracker was then opened.

This tool was used to perform the password cracking task using the hash obtained from the previous step.

**5. Paste the Hash**

The hash generated from the Hash Calculator was copied.

It was then pasted into the appropriate field in the Network Walks Password Cracker.

**6. Start Password Cracking**

After pasting the hash, the password cracking process was started.

The Password Cracker then attempted to identify the password associated with the supplied hash.

**7. Crack the Password**

After the cracking process was completed, the tool displayed the recovered password.

The recovered password was recorded for the next step.

**8. Test the Password on PDF 1**

The cracked password was used to open the first authorized password-protected PDF.

**Steps**

Open PDF 1.
Enter the recovered password.
Confirm that the password is accepted.
Verify that the PDF opens successfully.

**9. Test the Password on PDF 2**

The same recovered password was then tested against PDF 2.

Steps
Open PDF 2.
Enter the recovered password.
Confirm the password.
Verify that the PDF opens successfully.

**10. Test the Password on PDF 3**

Finally, the recovered password was tested against PDF 3.

**Steps**

Open PDF 3.
Enter the recovered password.
Confirm the password.
Verify that the PDF opens successfully.

**MODULE 2 — RESULT**

The second module demonstrated the complete Network Walks password cracking workflow:

PDF
 ↓
Network Walks Hash Calculator
 ↓
Hash Generated
 ↓
Network Walks Password Cracker
 ↓
Hash Pasted
 ↓
Password Cracked
 ↓
Password Recovered
 ↓
PDF 1
 ↓
PDF 2
 ↓
PDF 3


**EVIDENCE:**


<img width="867" height="687" alt="JTR - File upload" src="https://github.com/user-attachments/assets/774b7e78-5f99-4051-b74d-72c487351826" />
<img width="877" height="690" alt="Password cracking JTR" src="https://github.com/user-attachments/assets/cd056efc-2395-45e8-8c60-bb932a7fb568" />
<img width="1037" height="705" alt="CTF 3" src="https://github.com/user-attachments/assets/e140ef5d-913c-4355-941a-75533b7936ba" />
<img width="1052" height="772" alt="CTF 2 " src="https://github.com/user-attachments/assets/3bede974-083c-479c-a837-734c89bf2d67" />
<img width="892" height="547" alt="captured the flag" src="https://github.com/user-attachments/assets/8f234ff7-509a-4be2-8d0d-d7db0fae1355" />
<img width="1251" height="827" alt="Network walks hash calc and pwd cracking" src="https://github.com/user-attachments/assets/a68274e3-0f5d-4fcd-a597-0fb762cf8de3" />
<img width="1242" height="802" alt="Network walks hash calc and pwd cracking psf 3" src="https://github.com/user-attachments/assets/b5838291-a470-46ac-aaba-be5ac84ba120" />
<img width="1251" height="827" alt="Screenshot 2026-09-26 130937" src="https://github.com/user-attachments/assets/80f61bba-a231-4833-85dd-06c2bd89a2eb" />
<img width="1242" height="802" alt="Screenshot 2026-09-26 131209" src="https://github.com/user-attachments/assets/4f3df481-a1b1-4ef3-88e2-e27f2b37eaaf" />


After completing this project, I gained practical experience in:

Understanding password hashes
Working with password-protected PDF files
Using Network Walks security tools
Downloading and setting up John the Ripper
Working with John the Ripper binaries
Preparing hash files
Using password files / wordlists
Performing password recovery in an authorized lab
Verifying recovered passwords
Documenting cybersecurity practical tasks with screenshots and evidence


**Conclusion**

This project provided practical experience with password hashing and password recovery using Network Walks tools and John the Ripper.

The two modules covered the complete workflow from obtaining a hash to recovering the password and verifying the result against the authorized PDF files.

The project also helped build practical familiarity with command-line password recovery tools, hash handling, and documenting cybersecurity lab activities.

Disclaimer: All password cracking and password recovery activities documented in this repository were performed only on authorized Network Walks training files and lab environments.
