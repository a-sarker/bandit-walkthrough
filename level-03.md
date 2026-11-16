# Level 3

## Goal
Find and read a hidden file inside a directory.

## What I Used
- `cd` — change directory
- `ls -a` — list all files including hidden ones (files starting with `.`)
- `cat` — read the file

## Solution
`cd inhere`

`ls -a`

`cat ...Hiding-From-You`

## What I Learned
Files starting with a dot are hidden in Linux. Attackers hide malicious scripts and config files this way. As a SOC analyst, always use `ls -a` when investigating a server — `ls` alone will miss hidden files.
