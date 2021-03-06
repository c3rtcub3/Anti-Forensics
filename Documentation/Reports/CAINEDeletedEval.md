# Data Deletion Toolkit Evaluation Form

*Evaluator: Preston Wells*

*Forensics Toolkit: CAINE 7.0* 

Preston Wells

Capstone IASC-4580

Forensics Tool Analysis Team

### Purpose

The purpose of this is to test the analysis component of each of our forensic toolkits. Since the user story we will be testing is “As a **Computer Forensic Analyst**, I want to **detect and recover deleted data** so I can **support/define a suspect's intent**”, we will be analyzing and determining what the forensic toolkits miss or fail to recover. The deleted VM that we will be running our toolkits against has eight seperate files that were saved in various locations and then different tools were then used to deleted all eight of these files.

### File Deletion

File1_CC.txt - Text file deleted with CCleaner.

| Deleted File Not Found | Reference to File Found | Partial Recovery | Full Recovery |
|---|---|---|---|
|  |  **X(1)**  |   |   |

Comments:

File2_SD.txt - Text file deleted with SDelete.

| Deleted File Not Found | Reference to File Found | Partial Recovery | Full Recovery |
|---|---|---|---|
|   | **X(1)**  |   |   |

Comments:

File3_3P.txt - Text file deleted with Air Force 5020.

| Deleted File Not Found | Reference to File Found | Partial Recovery | Full Recovery |
|---|---|---|---|
|   | **X(1)**  |   |   |

Comments:

File4_7P.txt - Text file deleted with Schneier 7 pass.

| Deleted File Not Found | Reference to File Found | Partial Recovery | Full Recovery |
|---|---|---|---|
|   | **X(1)**  |   |   |

Comments:

File5_PCC.png - Image file deleted with CCleaner.

| Deleted File Not Found | Reference to File Found | Partial Recovery | Full Recovery |
|---|---|---|---|
|   | **X(1)**  |   |   |

Comments:

File6_PSD.png - Image file deleted with SDelete.

| Deleted File Not Found | Reference to File Found | Partial Recovery | Full Recovery |
|---|---|---|---|
|   | **X(1)**  |   |   |

Comments:

File7_P3P.png - Image file deleted with Air Force 5020.

| Deleted File Not Found | Reference to File Found | Partial Recovery | Full Recovery |
|---|---|---|---|
|   | **X(1)**  |   |   |

Comments:

File8_P7P.png - Image file deleted with Schneier 7 pass.

| Deleted File Not Found | Reference to File Found | Partial Recovery | Full Recovery |
|---|---|---|---|
|   | **X(1)**  |   |   |

Score:
8/24

Comments:
I was able to locate a tool in the toolkit that allowed me to parse a dd image and find the lnk files. This allowed me to find the lnk references for the previously deleted files but that was all I could find.

Proccess:
Create a Caine VM, and then attach the hard drive that I wanted to inspect to that VM. Once the machine was booted up, I used Guymager to carve the image and save the imaged in a .E0 format. Once the carver was done I then went into the version of autopsy that was on this tool kit and created a new case with the approriate images. Once that case was added, seeing as though for the purpose of this assignment we already new what the names of the files we were looking for were. I just used the file search, to search for the names of the appropriate files. But, because the files had not only their filename deleted they had been written over completely, the only thing that I could discover about this was the .lnks to where the previous files that I could no longer recover.
