<table style="width:100%; font-family: Verdana, Tahoma; border: none; border-collapse: collapse;">

<!-- University Logo -->
<tr>
<td colspan="3" style="text-align: center; vertical-align: middle; padding: 10px 0;">
<img src="https://www.kalasalingam.ac.in/wp-content/uploads/2022/02/Logo.png" 
alt="Kalasalingam Academy of Research & Education" 
style="height:80px; display:block; margin: 0 auto;">
</td>
</tr>

<!-- Department and School -->
<tr>
<td colspan="3" style="text-align: center; font-size: 18px; font-weight: bold; padding: 5px 0;">
Department of Computer Science Engineering | School of Computing
</td>
</tr>

<!-- Course and Section -->
<tr>
<td colspan="3" style="text-align: center; font-size: 16px; padding: 2px 0;">
Digital Forensics - 213CSE4307 | Lab Record | Section: 23S19 - Cybersecurity
</td>
</tr>

<!-- Experiment Info -->
<tr>
<td style="width:33%; text-align: left; padding-top: 10px;"><strong>Experiment No:</strong> 09</td>
<td style="width:34%; text-align: center; padding-top: 10px;">
<h3 style="margin: 0; font-family: Verdana, Tahoma;">Analyzing Suspicious Processes with Process Explorer </h3>
</td>
<td style="width:33%; text-align: right; padding-top: 10px;"><strong>Date:</strong> / /</td>
</tr>

</table>

<hr style="margin:10px 0;">
                     

**Overview**  
**Process Explorer** is a powerful Windows tool that provides detailed insights into running processes. It helps monitor system activity, troubleshoot issues, and detect potentially malicious or unusual processes. 

---

### Step 1: Download and Launch Process Explorer 

* **Get Process Explorer:**  
  Visit the Microsoft Sysinternals website and download the tool.
  link:-https://learn.microsoft.com/en-us/sysinternals/downloads/process-explorer
* **Extract Files:**  
  Unzip the downloaded package into a dedicated folder. 
* **Run as Administrator:**  
  Open the folder and launch `procexp64.exe` or `procexp.exe` by right-clicking and selecting **Run as Administrator**. 
  
<img width="1365" height="767" alt="Screenshot 2025-10-27 213149" src="https://github.com/user-attachments/assets/beb4f208-7054-4e4c-8cff-cec02e86344a" />

---

### Step 2: Explore the Interface 

Process Explorer displays processes in a hierarchical tree structure. Each process is **color-coded** based on its status:

| Color | Description |
| :--- | :--- |
| **Pink** | Suspended processes |
| **Light Blue** | Processes running under your account  |
| **Dark Blue** | System services or processes  |
| **Green** | Newly started processes  |
| **Red** | Recently terminated processes  |

---

### Step 3: Spotting Suspicious Processes 

To investigate potentially harmful processes:

1. **Check Unknown Processes:**  
   Look for unfamiliar names. Trusted processes usually come from known vendors like Microsoft, Adobe, or Intel. 
2. **Verify Digital Signatures:**  
   Right-click → **Properties** → **Image** tab. Check for a valid **Digital Signature**. Unsigned processes may be risky. 
3. **Examine File Paths:**  
   Check the **Path** under the Image tab. Legitimate system processes are usually in `C:\Windows\System32`. Running from temp or user folders is suspicious. 
4. **Monitor Resource Usage:**  
   Watch for processes consuming excessive CPU, memory, or disk resources without explanation. 
5. **Review Process Details:**  
   Lack of description or unclear company names can indicate a suspicious process. 
6. **Inspect Network Activity:**  
   Right-click → **Properties** → **TCP/IP** tab. Unexpected external connections require attention. 

---
<img width="787" height="591" alt="Screenshot 2025-10-27 213216" src="https://github.com/user-attachments/assets/c3817bb0-b496-4c92-9e17-d1ce1bd2b2a6" />



### Step 4: Research Suspicious Processes 

* Search the process name online (e.g., `cmd.exe`) to learn more about it. 
* Use databases like **VirusTotal** or **ProcessLibrary** to check for known malware. 


<img width="782" height="598" alt="Screenshot 2025-10-27 213346" src="https://github.com/user-attachments/assets/78182b1a-c7a4-4bc3-a5bf-2d08fcd4ce28" />

---

### Step 5: Handle Malicious or Unwanted Processes 

* **Terminate:** Right-click → **Kill Process** to stop it immediately.   
* **Suspend:** Right-click → **Suspend** to pause execution temporarily.  
* **Delete Source:** Locate the executable via its Path and remove it if confirmed malicious. 

---

<img width="776" height="584" alt="Screenshot 2025-10-27 213359" src="https://github.com/user-attachments/assets/7b652e63-1403-41ac-8b37-806d0f6bf431" />



<img width="773" height="590" alt="Screenshot 2025-10-27 213432" src="https://github.com/user-attachments/assets/ecab9c3e-3d93-4adc-9e6c-ba218db8ae63" />



---



### Step 6: Conduct a Full System Scan 

* Run a comprehensive antivirus scan. 
* Use malware removal tools (e.g., Malwarebytes or Windows Defender) for a thorough cleanup. 
<br>

<table style="width:100%; font-family: Verdana, Tahoma; border: none; border-collapse: collapse; margin-top:20px;">

<tr>
<td style="width:50%; text-align: left; padding: 10px;">
<strong>Student Name:</strong> Nischal S Tumbeti <br>
<strong>Register No:</strong> 99230041300
</td>

<td style="width:50%; text-align: right; padding: 10px;">
<strong>Verified by Faculty:</strong> Dr.K Venkatesh <br>
</td>
</tr>

</table>

<hr style="margin:10px 0;">
<p style="text-align:center; font-size:12px; font-family: Verdana, Tahoma; color:gray;">
Department of Computer Science and Engineering | School of Computing
</p>
