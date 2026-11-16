# Level 1

## Goal
Read a file called `-` (a dash).

## What I Used
- `cat ./-` — the `./` prefix tells Linux to treat `-` as a filename, not a flag

## Solution
`cat ./-`


## What I Learned
Attackers sometimes name malware or logs with special characters to make them harder to read. Knowing how to handle tricky filenames matters when you're investigating a compromised server.
