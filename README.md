# 📱 CTF Challenge 1: iOS IPA Reversing Walkthrough

Welcome to Challenge 1 of our iOS mobile CTF assignment. In this walkthrough, I’ll guide you through the process of extracting and analyzing an `.ipa` file, decrypting a suspicious key, and capturing our **first flag**. I also highlight some issues encountered while using **MobSF** for static analysis.

---

## 📦 Step 1: Download & Unzip the `.ipa` File

Begin by downloading the target `.ipa` file and unzipping it like a standard ZIP archive(I used 7-zip).

```bash
unzip Headbook-v1.0.ipa -d HeadbookExtracted
cd HeadbookExtracted/Payload


Payload/
└── Headbook.app/
    ├── Headbook                  
    ├── Info.plist
    ├── embedded.mobileprovision/
    ├── Main.storyboardc/
    └── PkgInfo


