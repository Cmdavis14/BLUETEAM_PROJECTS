# Windows Investigation Lab Solution

## Overview

This lab combines the analysis from **Windows Investigation 1** and **Windows Investigation 2** as part of a Digital Forensics project. The goal was to investigate user activity on a Windows system by analyzing various artifacts, including browser history, shortcuts, prefetch files, and jump lists. Through this investigation, we were able to reconstruct user actions, identify unauthorized activity, and locate potentially malicious files.

## Tools and Techniques

Throughout this investigation, the following tools and techniques were used:

- **Browser History Viewer (BHV)**: Used to load and analyze browsing history data, which allowed us to identify web browsers used, social media activity, cached images, and URLs visited.
- **Windows File Analyzer (WFA)**: Employed to analyze `.LNK` shortcut files, providing insights into downloaded files and interactions with potential malware.
- **PECmd.exe**: Utilized for parsing Windows Prefetch files, enabling us to track executable usage and confirm the involvement of certain files in suspicious activity.
- **JumpList Explorer**: This tool helped in analyzing Jump Lists, which log application usage and URLs accessed through certain applications.

## Investigation Process

### Part 1: Browser History Analysis

We started by opening **Browser History Viewer (BHV)** and loading the browsing history data to identify web browsers used by the user. Browsing data revealed that the user accessed several social media websites, which was against the company policy.

**Insert Screenshot Here: BHV showing list of web browsers used (sorted alphabetically).**

We then examined the URL column to identify specific sites visited by the user, focusing on identifying social media platforms. The history indicated visits to sites such as Discord, Facebook, Reddit, Twitter, and YouTube.

**Insert Screenshot Here: BHV URL column displaying social media sites accessed by the user.**

### Part 2: Cached Images Analysis

The cached images in BHV provided further insights. By filtering through the cached images at specific timestamps, we located an image related to an email, enabling us to view the subject line of the third email.

**Insert Screenshot Here: BHV showing cached image associated with email timestamp.**

### Part 3: Identifying Malicious Downloads

To trace any suspicious downloads, we searched the BHV records for files with extensions like `.exe` and `.zip`. We identified a ZIP file with an unusual name, which led us to investigate its origin. Based on timestamps and URLs, it appeared this file was downloaded from an external domain through a link likely embedded in an email.

**Insert Screenshot Here: BHV showing the suspicious ZIP file and associated URL.**

### Part 4: Analyzing Shortcuts with Windows File Analyzer

We used **Windows File Analyzer (WFA)** to examine `.LNK` files within the Shortcuts folder. These shortcuts contained information about files previously accessed on the system. Here, we identified a malicious file named **PlagueRat** within a ZIP file and located other files present in the same archive.

**Insert Screenshot Here: WFA showing shortcut file information with PlagueRat filename highlighted.**

### Part 5: Prefetch File Analysis with PECmd

Using **PECmd.exe**, we analyzed Prefetch files, particularly focusing on **CMD.EXE-89305D47.pf**. This analysis revealed that the **PlagueRat** batch file had been executed on the system. We also used specific keyword filters to trace applications that interacted with `plaguerat.ps1`.

**Insert Screenshot Here: PECmd output showing Prefetch entry for PlagueRat file.**

### Part 6: Jump List Analysis

The final stage involved analyzing the Jump Lists using **JumpList Explorer**. By looking for entries associated with web browsers, we found records indicating a visited website. This confirmed that Microsoft Edge was used to access specific online resources, including URLs potentially linked to malicious activity.

**Insert Screenshot Here: JumpList Explorer showing browser entries with website domain.**

## Summary

This investigation helped us understand the user's interactions with unauthorized websites, downloaded files, and potentially malicious activity on the system. By leveraging a variety of tools and parsing through artifacts like browser history, cached images, shortcut files, prefetch files, and jump lists, we were able to piece together a narrative of the user's actions.

This lab underscores the importance of examining multiple types of forensic evidence to accurately reconstruct events and identify security policy violations. The findings highlight potential gaps in corporate security practices regarding browsing policies and emphasize the necessity of continuous monitoring and education to mitigate risks.
