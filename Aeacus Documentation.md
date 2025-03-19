# AEACUS SCORE CHECKER DOCUMENTATION
**Tested and Documented by: Is-haq Abdulhanif Khatri**

*Automated Student Quiz Scoring Application*

## Overview

**AEACUS** is an automated scoring application developed by a high school student. It allows students to submit quizzes assigned by teachers, and the application evaluates scores automatically.

## Installation Guide

### Installing AEACUS on Linux Systems

#### Prerequisites

- Ensure your system has root access.

- Install dependencies as required (refer to the official repository).

### Installation Steps

**1.** **Download AEACUS** from the official repository: [Aeacus](https://github.com/elysium-suite/aeacus)

**2. Extract the Files**:

- Download `aeacus-linux.zip`, `source code (zip)`, and `source code (tar.gz)`.

**3. Modify Folder Permissions:**

`sudo chmod -R 777 /opt`

- Create a subfolder:

`mkdir /opt/Aeacus`

**4. Copy and Extract Files:**

- Move extracted files into `/opt/aeacus`.

**5. Create Configuration Files:**

- Navigate to the AEACUS folder:

`cd /opt/aeacus`

- Create `scoring.conf`:

`sudo nano scoring.conf`

- Paste the template from the [elysium-suite/aeacus](https://github.com/elysium-suite/aeacus) repository.

**6. Move Additional Required Files:**

- Copy ReadMe.conf from /opt/aeacus/misc/dev/ to /opt/Aeacus.

**7. Run AEACUS Commands:**
```
./aeacus --verbose score
```
```
./aeacus --verbose readme
```
**8. Resolve TeamID.txt Issue:**

- Locate the file in /misc/desktop/, copy the text, create a new nano file, paste contents, and save.

**9. Verify Installation:**
```
./aeacus --verbose check
```
```
./aeacus --verbose score
```
```
./aeacus --verbose readme
```

**10. Generate Scoring Report:**

`./aeacus --verbose release`

- The results will be generated in .html format on the desktop.

- Use Google Chrome to view the ScoringReport.html file.

### Installing AEACUS on Windows Systems

*Installation Steps*

**1.** **Download AEACUS** from the repository: [Aeacus](https://github.com/elysium-suite/aeacus)

**2. Extract Files:** Locate them in the Downloads folder.

**3. Run PowerShell Script:** Extract .zip and .tar.gz files to C:\.

**4. Copy Files:** Move extracted files to C:\Aeacus.

**5. Create Configuration Files:**

- Open `notepad`, create `scoring.conf`, and paste the template.

- Navigate to `misc\desktop`, copy `TeamID.txt`, and save it in `Aeacus` folder without `.txt` extension.

- Copy `ReadMe.conf` from `misc\dev\` and move it to the `Aeacus` folder.

**6. Run AEACUS Commands in PowerShell:**
```
./aeacus --verbose check
```
```
./aeacus --verbose score
```
```
./aeacus --verbose readme
```
```
./aeacus --verbose help
```
**7. Generate Scoring Report:**

`./aeacus --verbose release`

- Open the `.html` file via a browser.

## Troubleshooting and Common Issues

**1. Missing scoring.conf**

- Ensure `scoring.conf` exists in the AEACUS folder with the correct format.

**2. Missing `TeamID.txt`**

- Copy from `misc/desktop/` and ensure it is correctly saved.

**3. Missing `ReadMe.conf`**

- Copy from `misc/dev/` and place it in the AEACUS folder.

**4. `web.go` Requires Modification**

- Install [Go](https://go.dev/dl/) (`go build` in AEACUS directory).

- Edit `web.go`, `ReadMe.conf`, and `scoring.conf` using **Visual Studio 2022** for customization.

## Screenshots (Windows OS)
```
./aeacus --verbose check

./aeacus --verbose score

./aeacus --verbose readme

./aeacus --verbose help
```
----
# *End of Document*
