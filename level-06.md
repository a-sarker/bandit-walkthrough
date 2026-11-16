# Level 6

## Goal
Find a file somewhere on the entire server owned by user bandit7, group bandit6, and exactly 33 bytes.

## What I Used
- `find /` — search from the root of the filesystem
- `-user bandit7` — owned by this user
- `-group bandit6` — owned by this group
- `-size 33c` — exactly 33 bytes
- `2>/dev/null` — hide "Permission denied" errors

## Solution
`find / -user bandit7 -group bandit6 -size 33c 2>/dev/null`

`cat /var/lib/dpkg/info/bandit7.password`

## What I Learned
Searching an entire server by file ownership is a real SOC task. After a breach, you might run `find / -user compromised_account` to see every file that account touched. `2>/dev/null` is essential — without it, hundreds of
