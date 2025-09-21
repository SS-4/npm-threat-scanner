# 🚨 NPM Attack Scanner Toolkit - Sep 2025

**Detect the "Shai-Hulud" Supply Chain Attack on Windows Systems**

![PowerShell](https://img.shields.io/badge/PowerShell-%235391FE.svg?style=for-the-badge&logo=powershell&logoColor=white)
![Security](https://img.shields.io/badge/Security-Expert%20Verified-green?style=for-the-badge)

## 📦 What's Included

### 🔍 `NPM-Package-Scanner.ps1`
*Scans your projects for compromised NPM packages*
- ✅ Checks `package-lock.json` files
- ✅ Verifies against known malicious versions
- ✅ Fast results (seconds to minutes)
- ✅ Pinpoints infected projects

### 🔎 `Malware-Hash-Hunter.ps1`
*Finds the actual malicious payload on your system*
- ✅ Deep full-disk scan
- ✅ SHA-256 hash verification (100% accurate)
- ✅ Identifies the malicious `bundle.js` files
- ✅ Comprehensive threat detection

## 🚀 Quick Start

### Prerequisites
- Windows 10/11
- PowerShell 5.0+
- Administrator rights (for full scan)

### Installation
1. Download both `.ps1` files from this repository
2. Save them to your Desktop for easy access

## 🛠️ How to Run the Scanners
### Installation
```powershell
# Clone this repository
git clone https://github.com/SS-4/npm-threat-scanner.git
cd npm-threat-scanner
```
### For NPM-Package-Scanner.ps1:
1. **Right-click** on the `NPM-Package-Scanner.ps1` file
2. Select **"Run with PowerShell"**
3. Wait for the scan to complete (usually quick)
4. Review the results in the PowerShell window

### For Malware-Hash-Hunter.ps1 (ADMIN REQUIRED):
1. Place the file in the root of your C drive or any drive you want to scan.
2. Hold down the **SHIFT** key on your keyboard
3. While holding SHIFT, **Right-click** on the `Malware-Hash-Hunter.ps1` file
4. Select **"Copy as path"** from the menu
5. Click the **Start menu**, type **`PowerShell`**
6. **Right-click** on "Windows PowerShell" and select **"Run as administrator"**
7. In the blue admin window, type this and press **SPACEBAR**:
```powershell
Powershell -ExecutionPolicy Bypass -File "REPLACE-THIS-WITH-THE-FULL-PATH-TO-THE-PS1-FILES"
# EXAMPLE 1:
# Powershell -ExecutionPolicy Bypass -File "C:\NPM-Package-Scanner.ps1"
# EXAMPLE 2:
# Powershell -ExecutionPolicy Bypass -File "C:\Malware-Hash-Hunter.ps1"
```

8. Right-click to paste the path you copied earlier (replace "REPLACE-THIS-WITH-THE-FULL-PATH-TO-THE-PS1-FILES" with the actual path to your file, not the folder! ffs)
9. Press ENTER to start the deep scan
10. Wait 2-6 hours for complete system scanning

## 🎯 What It Finds
This toolkit detects:

✅ Compromised NPM packages (500+ affected)
✅ Malicious bundle.js payload variants
✅ Credential-stealing malware
✅ Supply chain attack indicators

## 📋 Results Interpretation
Package Scanner Results
- 🟢 Green output: No known compromised packages found
- 🔴 Red output: Infected packages detected - immediate action required

## Hash Hunter Results
- 🟢 Clean: No malicious files found
- 🔴 Infected: Malware detected - files listed for deletion

## 🚨 Emergency Actions
### If infection is detected:

IMMEDIATELY rotate all credentials:
NPM tokens (npmjs.com)
GitHub tokens (github.com)
AWS/Azure/GCP cloud credentials
All API keys and secrets
Clean infected projects:
Delete the node_modules folder
Delete the package-lock.json file
Manually edit package.json to use safe versions
Reinstall with: npm install --ignore-scripts
Delete any malicious files found by the hash hunter
Check your GitHub repositories for unauthorized changes
Ensure no repositories were made public
Check for strange GitHub Actions workflows

## 🛡️ Why This Works
Hash-based detection - No false positives
Comprehensive scanning - Full system coverage
Real-time verification - Against latest IOCs
Professional-grade - Enterprise-level detection

## 👨💻 Author
![Security](https://img.shields.io/badge/GitHub-SS--4-181717?style=flat&logo=github)

## 📚 Sources
IOC Data: Socket.dev Threat Intelligence
Attack Analysis: Truesec Security Research
Hash Verification: Multiple security vendors

## ⚠️ Disclaimer
This tool is provided for security purposes only. Use at your own risk.
The author is not responsible for any damages or data loss. Always
maintain backups and test in safe environments first.
Always run the hash hunter as Administrator for complete system access.
The deep scan will take several hours.

## Be patient and let it complete, only in silence! 😐


