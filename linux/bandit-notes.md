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

## Current Verified Progress

Current verified starting point: Bandit Level 13.

Completed:

- Level 8 -> Level 9
- Level 9 -> Level 10
- Level 10 -> Level 11
- Level 11 -> Level 12
- Level 12 -> Level 13

Level 11 -> Level 12 is not yet completed.

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
- Verifying progress by logging into the next level

## Investigation Workflow

For the layered Bandit challenge, the workflow was:

1. Identify the file type with `file`.
2. Choose the matching tool.
3. Decompress or extract.
4. Inspect the new file.
5. Repeat until the useful text is found.

This was a shift away from guessing commands and toward evidence-based troubleshooting.

## Reflection

Bandit is helping me build comfort with the Linux command line in a controlled environment. The main skill is not memorizing commands, but learning how to read a clue, choose a tool, test carefully, and verify the result.

## Next Step

Continue Bandit Level 13 using the same investigation-first approach.
