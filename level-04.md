# Level 4

## Goal
Find the one human-readable file among 10 files.

## What I Used
- `file ./-file*` — checks the type of every file at once using a wildcard
- `cat` — read the identified file

## Solution
`file ./-file*`

`cat ./-file07`

## What I Learned
The `file` command identifies what type of data a file contains — text, binary, executable, etc. On a real investigation, you'll have folders full of unknown files. Running `file *` is the fastest way to figure out what
