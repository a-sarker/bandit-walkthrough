# Level 0

## Goal
Log into the Bandit game server using SSH and find the password for the next level.

## What I Used
- `ssh` — connects to a remote server over an encrypted connection
- `cat` — prints the contents of a file

## Solution
ssh bandit0@bandit.labs.overthewire.org -p 2220

cat readme


## What I Learned
SSH is how security analysts remotely access servers to investigate incidents. The `-p` flag specifies a non-standard port. `cat` is the simplest way to read a file — you'll use it constantly when checking logs.
