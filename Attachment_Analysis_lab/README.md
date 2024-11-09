# Attachment Analysis Lab: Credential Harvester Investigation

## Objective
Investigate a phishing email attachment file to uncover information about a credential-harvesting attempt. Document key findings and answer specific questions regarding file details, hash, company impersonation, and more.

## Key Findings

1. **Phishing Email Attachment**
   - **Filename**: `MICROINV-US1070822.HTML`
   - **SHA256 Hash**: `0FC57290189ADECFE17F6BACBC515ED080CD63C54B282FDEF4EF3DFC598CDD1E`
   - **File Size**: `14.6 KB`

2. **Impersonated Company**
   - **Company Name**: Microsoft

3. **Phishing Target**
   - **Target Email Address**: `contact@securityblue.team`

4. **Microsoft Logo Filename in Phishing Page Source**
   - **Filename**: `microsoft_logo_ee5c8d9fb6248c938fd0dc19370e90bd.svg`

5. **Request URL Used in Credential Harvesting**
   - **Request URL**: `http://alia.typentfs.xyz/off.php?aaa=contact%40securityblue.team&ooo=test%40email.com&password=test&`

## Steps and Screenshots

### 1. Attachment File Analysis
![File Analysis Screenshot](screenshots/file_analysis.png)

### 2. Impersonation Web Page
![Impersonation Page Screenshot](screenshots/impersonation_page.png)

### 3. Autofilled Target Information
![Autofilled Target Screenshot](screenshots/autofilled_target.png)

### 4. Page Source and Microsoft Logo Filename
![Page Source Screenshot](screenshots/page_source.png)

### 5. Credential Harvesting Request URL
![Request URL Screenshot](screenshots/request_url.png)

## Conclusion
Summarize the phishing technique employed, the impersonation of a trusted company, and the targeting mechanism. Highlight the importance of careful analysis of email attachments.
