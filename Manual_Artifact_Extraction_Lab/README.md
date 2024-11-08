# Manual Artifact Extraction Lab

## Project Overview
The Manual Artifact Extraction Lab involved analyzing safe phishing emails to extract relevant artifacts manually. This lab demonstrates essential skills in phishing analysis, where manual artifact extraction methods are used to analyze suspicious emails when automated tools may not be available. Tools like Mozilla Thunderbird and Sublime Text 2 were used to view and analyze .eml files directly. PowerShell was used for hash calculations, and an online WHOIS lookup was performed to trace IP addresses back to their originating servers.

## Steps and Methods
1. Email Client Setup

- Opened each phishing email in Mozilla Thunderbird to review basic details, such as sender and recipient addresses, subject lines, and links.
- Email Artifact Collection with Sublime Text 2

2. Imported each .eml file into Sublime Text 2 to access detailed headers and metadata.
Collected specific information such as:
Sending Address: Extracted from the "From" field in the email header.
Recipient Address: Extracted from the "To" field.
Subject Line: Retrieved from the "Subject" field.
Received Date and Time: Retrieved from the "Date" field in the header.
Sending Server IP Address: Located in the header’s "Received" line, identifying the IP of the sending server.

3. WHOIS Lookup

For each IP address identified, used a WHOIS lookup service (whois.domaintools.com) to gather information on the sending server’s IP address, including:
Hostname: Identified through reverse DNS lookup, providing insights into the origin of the email.

4. URL and Root Domain Analysis

Inspected each email for URLs in the message body and extracted any hyperlinks found.
Documented both the full URL and root domain to identify potential malicious sites.

5. Attachment Analysis

Analyzed any attachments by performing the following:
Hash Calculation: Used PowerShell to generate MD5 and SHA-256 hashes of each attachment.
Filename Identification: Documented the file name for reference.

6. Final Documentation

Each artifact and its corresponding details were documented for reference. The information gathered provided a comprehensive profile of each phishing email, including sender identity, server origin, and attachment security information.

## Summary
This lab required manually collecting forensic data from phishing emails, including sender addresses, server IPs, URLs, and attachment hashes, using accessible tools. The exercise developed core skills in email artifact extraction, metadata analysis, and basic IP tracing, which are critical in incident response and threat analysis.

## Screenshots
Screenshots demonstrating key steps are located in the `screenshots` folder.
