# Linux Home Lab

This page documents my hands-on Linux practice through Ubuntu, command-line exercises, troubleshooting, and controlled cybersecurity learning labs.

## Current Environment

- Oracle VirtualBox
- Ubuntu 24.04.4 LTS
- Beginner command-line practice
- OverTheWire Bandit for safe Linux practice
## Completed Beginner Skills

- Opening and using the terminal
- Recognizing the shell prompt
- Checking the current directory with `pwd`
- Listing files with `ls`
- Moving between directories with `cd`
- Creating directories with `mkdir`
- Creating files with `touch`
- Writing text with `echo`
- Viewing file contents with `cat`
- Using SSH to connect to a remote practice server
- Leaving an SSH session with `exit`
- Reading error messages before changing commands
## Case 001: Incident Investigation

**Status:** Completed

**Goal:** Create and organize a simulated incident investigation using Ubuntu and the Linux command line.

**Skills Practiced**

- Linux navigation
- File management
- Evidence collection
- Basic incident investigation

**Summary**

Organized an investigation workspace, reviewed browser history and download activity, and identified indicators of a possible malware download.
**Explore:** [View Case 001](linux-%20cases/case-001-incident-investigation.md)
## Bandit Practice

**Status:** In progress

Current verified starting point: Bandit Level 16 -> 17.

Completed:

- Earlier Bandit basics through Level 8
- Level 8 -> Level 9
- Level 9 -> Level 10
- Level 10 -> Level 11
- Level 11 -> Level 12
- Level 12 -> Level 13
- Level 13 -> Level 14
- Level 14 -> Level 15
- Level 15 -> Level 16

**Explore:** [Bandit Notes](linux/bandit-notes.md)
## Recent Commands Practiced

- `cp`
- `mv`
- `mktemp`
- `tr`
- `xxd -r`
- `file`
- `gunzip`
- `bunzip2`
- `tar -xf`
- `cat`
- `scp -P 2220`
- `ssh -i`
- `chmod 600`
- `ls -l`
- `nc localhost 30000`
- `openssl s_client -connect localhost:30001`
- input/output redirection with `<` and `>`

## Current Linux Takeaway

The biggest improvement is using an investigation-first workflow: identify the file type or service requirement, choose the matching command, read errors carefully, and verify the result. The newest Bandit work added practice with connecting to an encrypted SSL/TLS service using OpenSSL.
## Next Linux Focus

- Continue Bandit Level 16 -> 17
- Practice local versus remote system awareness
- Continue learning permissions and secure file handling
- Continue documenting commands without publishing passwords or sensitive information
