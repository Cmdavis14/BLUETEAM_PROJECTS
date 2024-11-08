# BLUETEAM_PROJECTS

## Repository Overview
This repository contains a collection of blue team-focused labs and projects designed to demonstrate core cybersecurity skills, specifically around detection, analysis, and response. Each project includes detailed steps, screenshots, and insights into the tools and methods used to perform manual and automated security operations tasks. The repository showcases hands-on experience with incident analysis, artifact extraction, and forensic investigation techniques.

## Project List

1. **Manual Artifact Extraction Lab**
   - **Objective:** Analyze a two email attachment by extracting and verifying file hashes, reviewing email headers, and performing IP tracing.
   - **Methods:** Obtained SHA-256 and MD5 hashes, manually reviewed email headers in a text editor, and conducted a WHOIS lookup on the sender’s IP address.
   - **Skills Demonstrated:** Manual forensic artifact extraction, email header analysis, IP tracing.
   - **Files:** `Manual_Artifact_Extraction_Lab.md`  
   - **Screenshots:** Located in the `screenshots` folder.
   - **Summary:** This lab provides insight into the step-by-step processes for analyzing and identifying suspicious email artifacts.
   - [Manual Artifact Extraction Lab](Manual_Artifact_Extraction_Lab)

2. **Attachment Analysis Lab**
   - **Objective:** Investigate a phishing email attachment that impersonates Microsoft to harvest credentials.
   - **Methods:** Examined the attachment file’s properties, decoded the page source, identified autofilled recipient information, and traced the request URL used for credential harvesting.
   - **Skills Demonstrated:** Phishing analysis, file hash verification, source code analysis, identifying credential harvesting mechanisms.
   - **Files:** `Attachment_Analysis_Lab/README.md`  
   - **Screenshots:** Located in the `Attachment_Analysis_Lab/screenshots` folder.
   - **Summary:** This lab reveals the tactics behind a phishing attempt through file attachment analysis, emphasizing the importance of verifying email sources and inspecting file properties.
   - [Attachment Analysis Lab](Attachment_Analysis_lab/README.md)

3. **[Other Labs or Projects - Placeholder]**
   - Add details for other labs in the same format as you complete them.

## Repository Structure
