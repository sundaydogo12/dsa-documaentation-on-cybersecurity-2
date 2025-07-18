# dsa-documaentation-on-cybersecurity-2
## Digital Forensic Analysis Report

---

- Case Information

*Case Title:* Android Device Analysis – Case 2025-001  
*Case Number:* 2025-025  
*Date:* july 32, 2025  
*Prepared By:* sunday dogo  
agent  sam

---

- Executive Summary

This report presents the forensic analysis of an Android device image in ISO format. The image was processed using Autopsy, and key artifacts such as chat data, browsing history, and media metadata were recovered. The investigation focused on potential evidence of communication, location history, and deleted files------- Scope & Objectives

- To examine the contents of an Android image file (android_image.iso)
- To identify and extract user data such as messages, contacts, and images
- To recover deleted files and analyze media metadata
- To provide a summarized forensic overview for legal or investigative use

---

 🔧 Tools Used:

| Tool        | Version  | Purpose                     |
|-------------|----------|-----------------------------|
| Autopsy     | 4.21.0   | Forensic analysis           |
| Kali Linux  | 2024.4   | Host Operating System       |
| Sleuth Kit  | 4.12.1   | Backend processing engine   |
| dd        | Built-in | ISO to DD image conversion  |

- Methodology:

1. Received and verified the Android .iso file using SHA256 hashing.
2. Converted .iso to .dd format using dd command.
3. Loaded image into Autopsy as a disk image.
4. Scanned for web artifacts, images, app data, and deleted content.
5. Tagged and bookmarked relevant findings.
6. Exported final report and screenshots.

---

## 🗂 Findings

### 1. File System Overview

- File system: ext4  
- Partitions Detected: 3 (boot, system, data)  
- Image Size: 4.2 GB  
### 2. User Data Recovered

- *Contacts:* 48 contacts found in contacts2.db
- *SMS/MMS:* 152 text messages recovered
- *Call Logs:* 28 unique call entries

### 3. Web and App Artifacts

- *Chrome History:* Visited 83 websites  
- *WhatsApp DB:* Found in /data/com.whatsapp/databases/msgstore.db  
- *Telegram Cache:* Partial media cache recovered

### 4. Media Metadata (EXIF)

- 97 images found with GPS coordinates
- Device model: Samsung SM-A107F
- Camera app used: Android default

### 5. Deleted Files

- 41 deleted files recovered
- File types: .jpg, .mp4, .pdf
- Recovery success: 80%

### 6. Keyword Hits

- Searched terms: "fraud", "bitcoin", "password"
- 12 hits in SMS; 4 hits in WhatsApp

---

## 🖼 Screenshots

(Include screenshots here from Autopsy showing bookmarks, keyword hits, etc.)

---

-  Hash Verification

*Original File:* android_image.iso  
*SHA256 Hash:* f3b6c73f6b9e74d5d8c8cf1e13a3d7f4179876f09a12e7a8873b61e74aefb1ab  
*Hash Verified:* ✅ Yes

- ✅ Conclusion

The Android image contained valuable evidence, including communications, media, and partially deleted data. No evidence of external tampering or rooting was found. The extracted artifacts are consistent with regular device usage and support ongoing investigative leads.

---

-  Appendices

- Appendix A: Full file listing
- Appendix B: Autopsy HTML and CSV exports
- Appendix C: Chain of custody log (if applicable)

---

 final Report




