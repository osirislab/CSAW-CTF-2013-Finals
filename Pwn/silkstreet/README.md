# Silkstreet
## Author

## Points

## Category
Pwn
## Description
After silkroad got shut down, some competitors popped up.
This clone isn't even running over TOR... can you pop a shell and read the flag?
## Flag
`key{dr34d_pir8_1z_my_h0m3b0y}`
## Solution
`sploit.rb`
## Setup
RELRO           STACK CANARY      NX            PIE             RPATH      RUNPATH      FILE
No RELRO        No canary found   NX enabled    No PIE          No RPATH   No RUNPATH   silkstreet
there must be ASLR ON on this machine. Otherwise there would be no need to leak the heap addresses
## Notes
Hints:
its 2013, ALSR is on on the target machine...
Try to leak some pointers, br0
