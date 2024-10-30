# CTF Write-Up: CyberMaterialHavoc

## Introduction

This write-up discusses the challenge: **CyberMaterialHavoc** from the **Hack Havoc 2.0** CTF.

## Required Information

- **CTF Name:** Hack Havoc 2.0
- **Challenge Name:** CyberMaterialHavoc
- **Challenge Category:** Crypto
- **Challenge Points:** 150

## Content

The CyberMaterialHavoc challenge required decoding a message that was encrypted using three different ciphers. Here’s how I solved it:

### Step 1: Base92 Decoding
I began by decoding the original message using Base92, which gave:

    ZL{YfphiGdxdicgo_Yzkqu'i_Cmtg_Qfpdiscxawtiz_Xdxl_Khdxcltu}

### Step 2: Vigenere Cipher
Next, I applied the Vigenere Cipher with the key **CybermaterialHavoc** to the result from Step 1. This produced:

![](src\images\23.png)

    XN{XbyviNzgvirzo_Dliow'h_Yvhg_Xbyvihvxfirgb_Wzgz_Kozgulin}

### Step 3: Atbash Cipher
Finally, I used the Atbash cipher on the Vigenere result, which revealed the flag:

    CM{CyberMaterial_World's_Best_Cybersecurity_Data_Platform}

                 


![CTF Writeup by KoushikReddyB](src\images\Credits.png)