# CTF Write-Up: Hack Uncovered

## Introduction

This write-up discusses the challenge: **Hack Uncovered** from the **Hack Havoc 2.0** CTF.

## Required Information

- **CTF Name:** Hack Havoc 2.0
- **Challenge Name:** Hack Uncovered
- **Challenge Category:** OSINT
- **Challenge Points:** 40

## Content
The Case of the Missing Flag challenge involved uncovering a hidden flag within a disguised file. Here’s how I solved it:

### Step 1: Identifying the File Type
Using the command file abc.bat, I found that the file was actually an SVG image. I then renamed it to abc.svg to reflect the correct file type.

![](src\images\20.png)

### Step 2: Aligning the QR Code
I opened the SVG file in Photoshop (or Photopea online) and adjusted the QR code by aligning its top corner box into a perfect square.
![](src\images\21.png)

### Step 3: Scanning the QR Code
With the alignment corrected, the QR code became scannable, revealing the hidden flag.


## Flag: 
    CM{F0r3n3nic_1s_34sy}                 


