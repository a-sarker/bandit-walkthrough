# Level 9

## Goal
Find human-readable strings in a binary file, looking for the password marked with = signs.

## What I Used
- `strings` — extracts readable text from binary files
- `grep` — filters for lines containing "=="
- `|` — pipes strings output into grep

## Solution
`strings data.txt | grep "=="`

## What I Learned
Malware and binary files often contain readable strings — IP addresses, URLs, commands, credentials. The `strings` command pulls them out without opening the file. Malware analysts use this as a first step when examining a suspicious binary.
