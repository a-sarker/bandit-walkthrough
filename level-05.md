# Level 5

## Goal
Find a file across 20 subdirectories that is human-readable, 1033 bytes, and not executable.

## What I Used
- `find` with multiple conditions: `-type f` (file), `-size 1033c` (exact bytes), `! -executable` (not executable)

## Solution
`find inhere/ -type f -size 1033c ! -executable`

`cat inhere/maybehere07/.file2`

## What I Learned
The `find` command is one of the most powerful tools in Linux. In a SOC, you'll use it to search entire servers for suspicious files — by size, by owner, by modification time, by permissions. This level is exactly the kind of search you'd run during an incident: "find me every file modified in the last hour that's executable and owned by root."
