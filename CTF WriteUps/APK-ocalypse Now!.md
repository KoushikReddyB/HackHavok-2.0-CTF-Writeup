# CTF Write-Up: APK-ocalypse Now!

## Introduction

This write-up discusses the challenge: **APK-ocalypse Now!** from the **Hack Havoc 2.0** CTF.

## Required Information

- **CTF Name:** Hack Havoc 2.0
- **Challenge Name:** APK-ocalypse Now!
- **Challenge Category:** Mobile
- **Challenge Points:** 20

## Content
The **APK-ocalypse Now!** challenge required participants to decompile an Android application to find a hidden flag. The following steps outline the process I used to retrieve the flag:

### Step 1: Decompiling the APK
I used `apktool` to decompile the application with the following command:

```bash
apktool d -s hackhavoc.apk -o HackHavoc
```
This command decompiled the APK file and outputted the contents into a directory named HackHavoc.


![](src\images\4.png)

### Step 2: Locating the Flag
After decompiling, I opened the AndroidManifest.xml file and found the flag hidden as a comment within the file. The comment contained a Caesar cipher, which I then decoded to reveal the flag.

![](src\images\5.png)

### Step 3: Decoding with Caesar Cipher
Upon retrieving the flag, I noticed it was encoded with a Caesar cipher. I used a shift of 13 to decode it. For example, if the encoded flag was PZ{NOP}, the decoded flag would be CM{ABC} by shifting each letter back by 13 positions in the alphabet.

![](src\images\6.png)

## Flag: 
    CM{H1DD3N_7L4G_1N_M4NIF35T}



![CTF Writeup by KoushikReddyB](src\images\Credits.png)