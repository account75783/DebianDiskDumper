# DebianDiskDumper

**DebianDiskDumper** is a tiny Bash utility that makes *ddrescue-powered*, bit-perfect backups of CDs, DVDs, and Blu-ray discs. It even auto-detects the disc label, sanitises it into a safe filename, **and ejects the disc 30 seconds after the dump (unless you cancel).**

---

## ✨ Key features

| Feature | What it gives you |
|---------|------------------|
| **Auto-label → filename** | Reads the ISO-9660/UDF volume label and saves as `My_Disc.iso`. |
| **`ddrescue` imaging** | Sector-accurate, error-tolerant dumps—perfect for scratched media. |
| **One-keypress workflow** | Press **Enter** to accept the suggested name, or type your own. |
| **Auto-eject timer** | 30 s countdown after completion; press **N** to keep the disc loaded. |
| **Works everywhere** | Any Debian-based distro (Debian, Ubuntu, Mint, Pop!\_OS, Kali, etc.). |

---

## 🛠 Install prerequisites

```bash
sudo apt update
sudo apt install gddrescue eject   # util-linux & coreutils are already there

## Clone repo

git clone https://github.com/account75783/DebianDiskDumper.git
cd DebianDiskDumper
chmod +x diskdumper.sh
```
Tested on:

Ubuntu 24.04 LTS

CD's, DVD's, Not bluray yet (to do)

