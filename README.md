# BLUETEAM_PROJECTS

## Repository Overview
This repository contains a collection of blue team-focused labs and projects designed to demonstrate core cybersecurity skills, specifically around detection, analysis, and response. Each project includes detailed steps, screenshots, and insights into the tools and methods used to perform manual and automated security operations tasks. The repository showcases hands-on experience with incident analysis, artifact extraction, and forensic investigation techniques.

## Project List

1. **Manual Artifact Extraction Lab**
   - **Objective:** Analyzed two email attachments by extracting and verifying file hashes, reviewing email headers, and performing IP tracing.
   - **Methods:** Obtained SHA-256 and MD5 hashes, manually reviewed email headers in a text editor, and conducted a WHOIS lookup on the sender’s IP address.
   - **Skills Demonstrated:** Manual forensic artifact extraction, email header analysis, IP tracing.
   - **Files:** `Manual_Artifact_Extraction_Lab.md`
   - **Screenshots:** Located in the `screenshots` folder.
   - **Summary:** The lab provided insight into the step-by-step processes for analyzing and identifying suspicious email artifacts.
   - [Manual Artifact Extraction Lab](Manual_Artifact_Extraction_Lab/README.md)


2. **Attachment Analysis Lab**
   - **Objective:** Investigated a phishing email attachment that impersonated Microsoft to harvest credentials.
   - **Methods:** Examined the attachment file’s properties, decoded the page source, identified autofilled recipient information, and traced the request URL used for credential harvesting.
   - **Skills Demonstrated:** Phishing analysis, file hash verification, source code analysis, identifying credential harvesting mechanisms.
   - **Files:** `Attachment_Analysis_Lab/README.md`
   - **Screenshots:** Located in the `Attachment_Analysis_Lab/screenshots` folder.
   - **Summary:** The lab revealed the tactics behind a phishing attempt through file attachment analysis, emphasizing the importance of verifying email sources and inspecting file properties.
   - [Attachment Analysis Lab](Attachment_Analysis_Lab/README.md)

3. **Phishing Response Challenge Lab**
   - **Objective**: Identified and analyzed phishing emails, including email headers, sender details, and attachment analysis, to develop defensive measures.
   - **Methods**: Reviewed email headers, performed IP and reverse DNS lookups, and analyzed email attachments for malware or phishing signs. Proposed defensive strategies such as email filtering and user awareness             training.
   - **Skills Demonstrated**: Phishing email detection, header analysis, attachment analysis, incident response.
   - **Files**: `Phishing_Response_Challenge_Lab/README.md`
   - **Screenshots**: Located in the `Phishing_Response_Challenge_Lab/screenshots` folder.
   - [Phishing Response Challenge Lab](Phishing_Response_Challenge_Lab/README.md)

  
4.**Threat Intelligence Analysis with MISP Lab**
   - **Objective**: Conducted threat intelligence analysis using MISP to investigate ransomware, threat actor activities, DDoS attack strategies, and vulnerabilities in third-party software.
   - **Methods**: Explored MISP to research different ransomware types, analyzed the Turla Team threat actor, investigated DDoS events, and gathered intelligence on vulnerabilities affecting external vendors.
   - **Skills Demonstrated**: Threat intelligence gathering, ransomware analysis, threat actor research, vulnerability analysis, DDoS investigation.
   - **Files**: `Threat_Intelligence_MISP_Lab/README.md`
   - [Threat Intelligence Analyis with MISP Lab](Threat_Intell_Using_MISP/README.md)



 5. **Identifying_File_Systems_FTKImager**
   - **Objective**: Analyzed three disk images (`carve1.img`, `carve2.img`, and `disk1.img`) to identify the file systems used by the imaged computers.
   - **Methods**: Used **FTK Imager** to import and analyze disk images. For each image, I examined the file system properties and identified the file system types (NTFS, FAT32, and Linux). This process involved importing each disk image into FTK Imager, reviewing the          properties tab, and identifying the file system structure for forensic investigation.
   - **Skills Demonstrated**: Disk image analysis, file system identification (NTFS, FAT32, Linux), using FTK Imager for forensic analysis, and understanding forensic methodologies for file system determination.
   - **Files**: `Disk_Image_Analysis_Lab/README.md`
   - [Identifying File systems using FTK Imager](Identifying_File_Systems_FTKImager/README.md)


6.  **Metadata_Analysis_and_File_Carving_Lab**

- **Objective**: Performed metadata analysis and file carving on digital files to retrieve hidden data and identify essential metadata details. The tasks involved analyzing metadata of files (`dummy.pdf` and `picture.jpg`) and carving a deleted image from a disk image                     (`carve1.img`).
- **Methods**: Utilized **exiftool** to extract metadata details from files, including identifying the author of a PDF and the camera model used for a photo. Used **Scalpel** for file carving, configuring it to recover deleted images from a disk image. This process                      included modifying `scalpel.conf`, creating an output directory for recovered files, and verifying the integrity of the carved image with an MD5 hash.
- **Skills Demonstrated**: Metadata Extraction, File Carving with Scalpel, Hash Verification, Forensic Methodologies.
- **Files**:`Metadata_and_File_Carving/README.md`
- [Metadata Analysis and File Carving Lab](Metadata_and_File_Carving/README.md)


## Repository Structure
