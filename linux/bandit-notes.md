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

Current verified state: logged in as `bandit11`.

Completed:

- Level 8 -> Level 9
- Level 9 -> Level 10
- Level 10 -> Level 11

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

## Concepts Practiced

- Reading a level goal carefully
- Matching a clue to a command
- Using pipes to send one command's output into another command
- Filtering large output into useful results
- Decoding encoded text
- Verifying progress by logging into the next level

## Reflection

Bandit is helping me build comfort with the Linux command line in a controlled environment. The main skill is not memorizing commands, but learning how to read a clue, choose a tool, test carefully, and verify the result.

## Next Step

Resume Bandit Level 11 -> Level 12.

Completion evidence will be successfully logging in as `bandit12`.
