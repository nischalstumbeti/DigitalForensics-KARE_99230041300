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
<td style="width:33%; text-align: left; padding-top: 10px;"><strong>Experiment No:</strong> 08</td>
<td style="width:34%; text-align: center; padding-top: 10px;">
<h3 style="margin: 0; font-family: Verdana, Tahoma;">Detect Hidden Data in Images Using StegExpose</h3>
</td>
<td style="width:33%; text-align: right; padding-top: 10px;"><strong>Date:</strong> / /</td>
</tr>

</table>

<hr style="margin:10px 0;">

---

##  Aim

To detect hidden data in image files using **StegExpose**, a steganography analysis tool.

---

##  Description

**StegExpose** is a Java-based forensic tool that identifies potential hidden data in images. It analyzes the **statistical properties** of image files to estimate a “suspect score,” helping investigators determine whether steganography is likely present.

The higher the suspect score, the more probable it is that hidden data exists.

---

##  Prerequisites

Before starting, ensure the following software and files are prepared:

###  Software Requirements

1. **Java Development Kit (JDK 8 or higher)**
   StegExpose is Java-based, so `java` and `javac` must be installed.

   **Windows:**

   ```bash
   choco install openjdk
   ```

   **Ubuntu/Linux:**

   ```bash
   sudo apt update
   sudo apt install default-jdk
   ```

   **macOS:**

   ```bash
   brew install openjdk
   ```

    Verify installation:

   ```bash
   java -version
   javac -version
   ```

2. **Apache Commons Math Library**

   * Required dependency: `commons-math3-3.1.1.jar`
   *  Download from: `https://archive.apache.org/dist/commons/math/binaries/commons-math3-3.1.1-bin.zip`

3. **StegExpose Source Code**

   * Clone or download from GitHub: `https://github.com/b3dk7/StegExpose`

   ```bash
   git clone https://github.com/b3dk7/StegExpose.git
   ```

###  Environment Setup

Place all files in a single working directory (e.g., `C:\StegExpose\`) and navigate there using Command Prompt (Windows) or Terminal (Linux/macOS):

```bash
cd C:\StegExpose
```

---

##  Step 1 — Compile the Source Code

Compile the Java files with the required dependency:

```bash
javac -cp commons-math3-3.1.1.jar -source 1.8 -target 1.8 *.java
```

<img width="1111" height="619" alt="Screenshot 2025-10-27 203134" src="https://github.com/user-attachments/assets/a6435011-8c99-4f60-84dd-ca634c1a54e7" />



 Note: Ignore warnings like `RSAnalysis.java uses unchecked or unsafe operations`. Compilation is successful if `.class` files are generated.

---

##  Step 2 — Create the Executable JAR
By using Notepad
Create a file named `manifest.mf` in the same folder:

```
Main-Class: StegExpose
```

<img width="1338" height="601" alt="Screenshot 2025-10-27 211406" src="https://github.com/user-attachments/assets/f23b65e5-8435-41bb-b31c-d6be936a6b1d" />



Build the JAR:

```bash
jar cfm StegExpose.jar manifest.mf *.class
```




 You now have `StegExpose.jar` ready to use.

---

##  Step 3 — Run StegExpose

```bash
java -jar StegExpose.jar "C:\StegExpose\testFolder"
```
<img width="1173" height="550" alt="Screenshot 2025-10-27 202956" src="https://github.com/user-attachments/assets/db2a4ea6-a5ff-4c55-a87f-ceee85fe8ac0" />

---

##  Step 4 — Example Output


| Hidden Bytes   | Meaning                             |
| -------------- | ----------------------------------- |
| < 10,000       | Likely clean (no hidden data)       |
| 10,000–100,000 | Possibly contains hidden data       |
| > 100,000      | Highly likely steganography present |

---

##  Step 5 — Analyze and Verify Results

The tool lists images with potential hidden data and estimates the approximate size. Further validation can be done using tools such as:

* StegSolve
* OpenStego
* zsteg
* Binwalk

---

##  Optional — Export Results Automatically

Generate a results file for easier review:

```bash
java -jar StegExpose.jar "C:\madhi\StegExpose\testFolder" fast 0.3 results.csv

```

## Conclusion

* Successfully compiled and executed StegExpose
*  Detected images containing potential hidden data
*  Interpreted results and exported findings

Hidden data in image files was successfully detected using StegExpose. 

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
