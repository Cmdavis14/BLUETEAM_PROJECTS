# Metadata and File Carving Lab

## Overview

This lab was designed to practice analyzing file metadata and retrieving hidden or deleted data using file carving techniques. The tasks involved analyzing metadata from a PDF and an image, as well as recovering a deleted image from a disk image using the tool `scalpel`. This exercise enhanced my familiarity with metadata extraction, file carving, and the use of terminal-based forensic tools.

## Summary

Through this lab, I developed skills in:
- Extracting metadata from various file types using `exiftool`
- Setting up and configuring `scalpel` to recover deleted files from disk images
- Navigating and managing files in a Linux environment

## Steps

### 1. Set Up Terminal in Lab Directory
   - I started by opening a terminal session in the `Metadata and File Carving` directory on the Desktop. This was essential for running the metadata and carving commands on the files located in this folder.

### 2. Metadata Analysis Using `exiftool`
   - **Description**: Used `exiftool` to analyze metadata in files to extract specific details.
   - **Process**:
     - Ran `exiftool` on a PDF file to identify metadata fields like the author.
     - Ran `exiftool` on an image file to retrieve details such as the camera model.
   - **What I Learned**: This exercise introduced me to `exiftool`, a powerful utility for examining and extracting metadata, which is useful in digital forensics to gather information from file properties.

   **Screenshot**: Insert screenshots here showing terminal output from the `exiftool` commands.

### 3. File Carving with `Scalpel`
   - **Description**: Configured and used `scalpel` to recover a deleted image file from an NTFS-formatted disk image.
   - **Process**:
     - Made a copy of the default `scalpel.conf` file and modified it to specify image file formats (`jpg` and `gif`) by uncommenting related lines.
     - Created a dedicated output directory for the carved files.
     - Used `scalpel` with the configured file to search and extract image files from the disk image (`carve1.img`).
     - Calculated the MD5 hash of the recovered image to verify the file’s integrity.
   - **What I Learned**: This step taught me about file carving, a technique used in data recovery and forensics to extract files from disk images based on file signatures. Configuring `scalpel` gave me hands-on experience with modifying configuration files and using Linux commands to manage permissions and navigate the filesystem.

   **Screenshot**: Insert screenshots here showing steps in the terminal, including:
   - The edited `scalpel.conf` file
   - Commands run for carving and MD5 hash calculation
   - The output of the recovered file's hash calculation

## Key Takeaways

- **File Metadata Analysis**: `exiftool` is an effective tool for identifying key metadata, which can be critical in digital investigations for understanding file origins.
- **File Carving Techniques**: `scalpel` is useful for recovering deleted files by identifying file headers and footers, even from formatted drives.
- **Linux Terminal Proficiency**: The lab improved my skills in using the Linux terminal, editing configuration files, handling permissions, and organizing output data.

## Conclusion

This lab provided practical experience in digital forensics, focusing on metadata analysis and file carving. I now have a better understanding of how to retrieve hidden data and analyze file properties, skills which are essential for investigations and data recovery.

---

