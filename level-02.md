# Level 2

## Goal
Read a file with spaces and dashes in the name.

## What I Used
- Quotes around the filename to handle spaces
- `./` prefix to handle the leading dashes

## Solution
`cat ./'--spaces in this filename--'`

## What I Learned
Wrap filenames with spaces in quotes. Combine with `./` when the name starts with special characters. Log files and evidence on compromised systems can have weird names — you need to handle them without panicking.
