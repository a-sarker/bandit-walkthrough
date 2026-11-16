# Level 10

## Goal
Decode a base64-encoded file to reveal the password.

## What I Used
- `base64 -d` — decodes base64-encoded data back to plain text

## Solution
`base64 -d data.txt`

## What I Learned
Base64 is everywhere in security — email attachments, web tokens, obfuscated malware payloads, encoded PowerShell commands. Attackers use it to hide malicious content in plain sight. When you see a long string of letters, numbers, and ending in = or ==, it's probably base64. Decoding it is step one of investigating it.
