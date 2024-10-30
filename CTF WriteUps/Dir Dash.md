# CTF Write-Up: Dir Dash

## Introduction

This write-up discusses the challenge: **Dir Dash** from the **Hack Havoc 2.0** CTF.

## Required Information

- **CTF Name:** Hack Havoc 2.0
- **Challenge Name:** Dir Dash
- **Challenge Category:** Web
- **Challenge Points:** 60

## Content
The Dir Dash (Web) challenge involved exploring directories and testing file extensions to uncover a hidden flag.

### Step 1: Navigate to robots.txt
First, I visited http://edition1.ctf.cybermaterial.com/ and accessed robots.txt, where I discovered a hash: c5ba7ff1883453170f7590fa689f1f48.

![](src\images\28.png)

### Step 2: Brute-Force File Extensions
Next, I brute-forced different file extensions to locate a hidden file. After trying various possibilities, I found a valid result with the .aspx extension.

![](src\images\29.png)

## Flag: 
    CM{3xten5i0n5_w45_CR4zY}          
![CTF Writeup by KoushikReddyB](src\images\Credits.png)