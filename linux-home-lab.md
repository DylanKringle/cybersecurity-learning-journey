# Linux Home Lab

This page documents my hands-on Linux practice using Ubuntu. Rather than only learning individual commands, I complete realistic cybersecurity labs that reinforce Linux fundamentals while simulating common security and system administration tasks.

---

# Lab 1: Incident Investigation ✅

**Status:** Completed

## Objective

Create and organize a simulated incident investigation using the Linux command line while practicing basic Linux navigation and file management.

---

## Investigation Scenario

A user reported downloading a suspicious file and unusual system behavior. The objective was to organize evidence, create an investigation workspace, review collected artifacts, and identify the most suspicious activity.

---

## Lab Structure

```text
investigation-001/
├── evidence/
│   ├── browser-history.txt
│   ├── downloads.log
│   └── suspicious-file.txt
├── notes/
├── screenshots/
└── report.txt
```

---

## Evidence Reviewed

### Browser History

- google.com
- nyu.edu
- gmail.com
- freegift.ru
- bank-login-security.com
- youtube.com

### Downloads

- chrome.exe
- invoice.pdf
- free_game.exe
- holiday_photo.jpg

### Suspicious File

```
Possible Malware

Downloaded From:
freegift.ru

Status:
Unknown
```

---

## Investigation Findings

The suspicious browsing activity led to **freegift.ru**. The most suspicious downloaded file was **free_game.exe**, and the suspicious file referenced the same website, suggesting a possible malware download.

---

## Linux Commands Practiced

- `pwd`
- `ls`
- `cd`
- `cd ..`
- `mkdir`
- `touch`
- `nano`
- `cat`
- `rm`

---

## Lessons Learned

- Learned the difference between files and directories.
- Practiced navigating the Linux filesystem using both relative and absolute paths.
- Created, edited, and viewed files from the terminal.
- Used Linux commands within a realistic cybersecurity investigation instead of isolated command exercises.

---

## Reflection

This was my first Linux security lab. Instead of memorizing commands, I used Linux to complete a simulated incident investigation by organizing evidence, reviewing artifacts, and identifying suspicious activity. This made the command line feel much more practical and helped reinforce Linux fundamentals through hands-on problem solving.
