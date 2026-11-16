# Level 8

## Goal
Find the only line that appears once in a file where every other line is repeated.

## What I Used
- `sort` — sorts lines alphabetically so duplicates are grouped together
- `uniq -u` — prints only lines that appear exactly once
- `|` (pipe) — sends output of one command as input to the next

## Solution
`sort data.txt | uniq -u`

## What I Learned
Piping commands together is how Linux gets powerful. Each command does one small job — sort arranges, uniq filters — and the pipe chains them. In SOC work, you'll chain 3-4 commands together regularly: grep for an IP, sort the results, count occurrences, find the outlier.
