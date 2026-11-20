# Password Auditing with John the Ripper in Kali Linux

A quick demonstration of installing and running [John the Ripper](https://www.openwall.com/john/) on [Kali Linux](https://www.kali.org/tools/john/) to test and audit password hash strength.

## Overview
[John the Ripper](https://www.openwall.com/john/) is an open-source password security auditing and recovery tool. This repository documents basic installation, wordlist usage, and hash cracking output in a local lab environment.

## Setup & Usage

1. **Install John the Ripper** (if not pre-installed):
   ```bash
   sudo apt update && sudo apt install john -y
   ```

2. **Run a wordlist attack against a hash file:**
   ```bash
   john --wordlist=/usr/share/wordlists/rockyou.txt hashes.txt
   ```

3. **View cracked passwords:**
   ```bash
   john --show hashes.txt
   ```

## Disclaimer
This project is for educational purposes and authorized security testing only.
