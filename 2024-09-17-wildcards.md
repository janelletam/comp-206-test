# Shell wildcards

'*' match everything
- E.g. `ls *c` finds any file ending in c

'?' matches single character
- E.g. `ls bob.d?c` finds any file ending in bob.d[character]c where
? can be any character from [0, 9] and [a, z]

; and && join programs tgoether and || is an or symbol
- E.g. `ls; ls example (run ls, and then run ls example)`
- E.g. exit 0 || echo hello world), exit 0 returns true, so program doesn't return echo hello world. (e.g. exit 1 || echo hello world), exit 1 returns false so program will run hello world

'[]' matches any character in the square brackets
- E.g ls bob.d?[a-zA-Z] (e.g. lists all files that are in the format bob.d[one character][any character from a-z and A-Z)

**Wildcards are interpreted by the SHELL. NOT the program we're running**
