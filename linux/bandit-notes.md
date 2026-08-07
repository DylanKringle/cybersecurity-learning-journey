# OverTheWire Bandit Notes

These notes document command-line practice from OverTheWire Bandit. Passwords are intentionally excluded.

## Safety Rule

Do not store or publish:

- Bandit passwords
- Real passwords
- API keys
- SSH private keys
- Tokens
- Personal credentials
- Private-key contents

## Current Verified Progress

Current verified starting point: Bandit Level 15 -> 16.

Completed:

- Earlier Bandit basics through Level 8
- Level 8 -> Level 9
- Level 9 -> Level 10
- Level 10 -> Level 11
- Level 11 -> Level 12
- Level 12 -> Level 13
- Level 13 -> Level 14
- Level 14 -> Level 15

Bandit Level 15 -> 16 and later are not yet documented as complete.

## Earlier Bandit Progress: Levels 0-7

**Status:** Completed before detailed note-taking became consistent

These early levels introduced basic command-line investigation and remote Linux practice. Detailed notes begin at Level 8, where documentation became more consistent.

### Skills Introduced

- Connecting to a remote Linux server with SSH
- Navigating the filesystem
- Reading files from the command line
- Listing directory contents
- Finding hidden files
- Handling unusual filenames
- Checking file types
- Using clues from the level goal instead of guessing
- Verifying progress by logging into the next level

### Documentation Note

This section is a backfilled summary. It records the progression honestly without pretending to have detailed notes for every early level.

## Recent Bandit Milestones

### Level 13 -> Level 14

**Concept:** SSH private-key authentication

Skills practiced:

- Identified an OpenSSH private key with `file`
- Distinguished the remote Bandit server from the local Ubuntu VM
- Copied a key file securely with `scp`
- Corrected the port flag difference between `ssh -p` and `scp -P`
- Used `chmod 600` to restrict private-key permissions
- Verified permissions with `ls -l`
- Used `ssh -i` to authenticate with an identity file

Important lesson:

SSH private keys must have restrictive permissions. The private-key permission warning was useful because it explained exactly why the key was ignored.

### Level 14 -> Level 15

**Concept:** localhost, ports, and Netcat

Skills practiced:

- Read the level goal carefully
- Used `cat` to read the current-level password file without publishing it
- Learned that `localhost` means the current machine
- Learned that a port identifies a specific service/process endpoint
- Connected to a TCP service with `nc localhost 30000`
- Corrected a port typo from `3000` to `30000`
- Used the service response as verification

Important lesson:

Netcat can connect directly to a network service. When the shell prompt disappears, the command may be waiting for input to send to that service.

## Commands Practiced

### `sort`

Used to organize lines so duplicate or related lines can be grouped together.

### `uniq -u`

Used after sorting to identify a line that appears only once.

Example pattern:

```bash
sort data.txt | uniq -u
```

### `strings`

Used to extract human-readable text from a file that may contain unreadable or binary-looking data.

### `grep`

Used to filter command output for a specific clue or pattern.

Example pattern:

```bash
strings data.txt | grep =
```

### `base64 -d`

Used to decode Base64-encoded text.

Example pattern:

```bash
base64 -d data.txt
```

### `tr`

Used to translate or substitute characters.

### `xxd -r`

Used to reverse a hexdump back into binary data.

### `file`

Used to identify what type of file is being inspected before choosing the next command.

### `gunzip`

Used to decompress gzip-compressed files.

### `bunzip2`

Used to decompress bzip2-compressed files.

### `tar -xf`

Used to extract files from a tar archive.

### `mktemp`

Used to create a temporary working directory.

### `cp` and `mv`

Used to copy, move, and rename files during investigation.

### `scp -P 2220`

Used to securely copy files over SSH while specifying the SSH port.

### `ssh -i`

Used to authenticate with a private identity file.

### `chmod 600`

Used to restrict a private key so only the owner can read and write it.

### `ls -l`

Used to inspect Unix file permissions.

### `nc localhost 30000`

Used to connect to a local TCP service with Netcat.

### Input and Output Redirection

Practiced using `<` and `>` to control input and output.

## Concepts Practiced

- Reading a level goal carefully
- Matching a clue to a command
- Using pipes to send one command's output into another command
- Filtering large output into useful results
- Decoding encoded text
- Identifying file types before choosing tools
- Reversing a hexdump
- Decompressing layered archive formats
- SSH private-key authentication
- Secure file transfer with `scp`
- Linux file permissions
- Local versus remote systems
- Localhost and ports
- Connecting to services with Netcat
- Verifying progress by logging into the next level

## Investigation Workflow

The general Bandit workflow is:

1. Read the level goal.
2. Inspect available files and hints.
3. Identify file types or service requirements.
4. Choose the tool that matches the evidence.
5. Read errors carefully.
6. Verify the result before recording progress.

This keeps the practice focused on reasoning instead of memorizing commands.

## Next Step

Continue Bandit Level 15 -> 16 using the same investigation-first approach.
