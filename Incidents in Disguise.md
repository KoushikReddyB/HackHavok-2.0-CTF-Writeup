# CTF Write-Up: Incidents in Disguise

## Introduction

This write-up discusses the challenge: **Incidents in Disguise** from the **Hack Havoc 2.0** CTF.

## Required Information

- **CTF Name:** Hack Havoc 2.0
- **Challenge Name:** Incidents in Disguise
- **Challenge Category:** Stego
- **Challenge Points:** 40

## Content
The Stego: Incidents in Disguise challenge required uncovering a hidden flag using hints and steganography. The following steps outline my approach:

### Step 1: Following the Discord Hint
I began by following the Discord hint, "amos," which suggested that the hidden information could be accessed using the steghide tool. So i used grep tool to search for "amos" in entire wordlist
```bash
grep "amos" /usr/share/wordlists/rockyou.txt
```
![](src\images\7.png)

### Step 2: Manual Brute Force
Given the hint that the password would be found towards the end, I manually checked the last entry from my grep results and discovered that the correct password was "*7¡Vamos!"
![](src\images\8.png)

## Flag: 
    CM{Bru73_f0rc3_i5_b35t}                 


![CTF Writeup by KoushikReddyB](src\images\Credits.png)