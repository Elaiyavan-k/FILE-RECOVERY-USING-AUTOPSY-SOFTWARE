# FILE-RECOVERY-USING-AUTOPSY-SOFTWARE
# Name: ELAIYAVAN K
# Reg.no: 212224100015


## AIM
To use **Autopsy Digital Forensics Tool** to retrieve deleted files from a disk image.

---

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tool**: [Autopsy Digital Forensics](https://www.autopsy.com/)  
- **Test Data**: Disk image file (`disk.dd`, `disk.img`, `.E01`)

---

## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Install Autopsy]
    B --> C[Create New Case in Autopsy]
    C --> D[Add Data Source: Disk Image]
    D --> E["Run File System & Data Recovery Modules"]
    E --> F[Locate Deleted Files in Results]
    F --> G[Recover and Export Deleted Files]
```
## DESIGN STEPS:
### Step 1:
Open Autopsy and create a new case with appropriate case details.

### Step 2:
Add a disk image as a data source and let Autopsy analyze the content.

### Step 3:
Navigate to the "Deleted Files" section in Autopsy and examine or recover the deleted files.

## PROGRAM:
### Install Autopsy
```bash
# Download Autopsy from:
# https://www.autopsy.com/
# Install following the setup wizard.
```
### Create a New Case
```
# File → New Case
# Enter Case Name: Deleted_File_Recovery
# Choose Base Directory: C:\Cases\Deleted_File_Recovery
# Click Finish
```
### Add Disk Image
```
# Add Data Source → Disk Image or VM File
# Browse to: C:\forensics\disk.dd
# Click Next
```
### Run Ingest Modules
```# Select:
# - File System Analysis
# - Keyword Search (optional)
# - Data Recovery / Carving
# Click Finish
```
### Locate Deleted Files
```
# Navigate to 'Deleted Files' section in the tree view
# Review metadata (size, hash, timestamps)
```
### Export Deleted Files
```
# Right-click → Extract File(s)
# Save to: C:\forensics\Recovered_Files\
```

## OUTPUT:
Recovered Deleted File List and Details

<img width="1600" height="847" alt="WhatsApp Image 2026-08-22 at 12 35 28 PM" src="https://github.com/user-attachments/assets/f641d020-a5cf-4f8a-b403-31674d738c79" />

<img width="1600" height="848" alt="WhatsApp Image 2026-08-22 at 12 37 47 PM" src="https://github.com/user-attachments/assets/91879132-273e-4a7a-93b3-42a11d3432f8" />

<img width="1600" height="851" alt="WhatsApp Image 2026-08-22 at 12 39 58 PM" src="https://github.com/user-attachments/assets/567316da-e765-451c-bc7c-1da915980fde" />

<img width="1600" height="850" alt="WhatsApp Image 2026-08-22 at 1 40 42 PM" src="https://github.com/user-attachments/assets/d18c3f04-37e9-4dc2-af05-e86022c9c336" />

<img width="1600" height="855" alt="WhatsApp Image 2026-08-22 at 2 02 12 PM" src="https://github.com/user-attachments/assets/9ca7a0f7-50db-4d95-98a7-633c077518c4" />

<img width="1600" height="845" alt="WhatsApp Image 2026-08-22 at 3 24 13 PM" src="https://github.com/user-attachments/assets/cdab3681-6e03-418a-b6de-299f364a4643" />

<img width="1600" height="846" alt="WhatsApp Image 2026-08-22 at 3 23 19 PM" src="https://github.com/user-attachments/assets/98879123-2dbd-430d-8e52-7b8307ae3346" />


## RESULT:
Deleted files were successfully retrieved and analyzed using Autopsy.
