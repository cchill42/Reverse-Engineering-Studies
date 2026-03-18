# Table of Contents
- [Overview](#Overview)
- [Usage](#Usage)

# Overview
This is the first tool I ever learned about regarding reverse engineering. First learning it, it seems it is just a way to find string literals in binary files. 

So far, I have not really dived deeply into this tool, but I do find it to be very useful already.

# Usage
Looking at this usage of it on a basic executable CrackMe, It can find method calls and literals used in printing. (As shown in the "try again!" and "Nice Job!!" messages)
```
ff.
u/H
u~H
uTH
<@u-H
AWAVI
AUATL
%f+
-f+
t 1
[]A\A]A^A_
USAGE: %s <password>
try again!
Nice Job!!
flag{%s}
;*3$"
GCC: (Debian 7.3.0-25) 7.3.0
crtstuff.c
deregister_tm_clones
__do_global_dtors_aux
completed.7090
```

And here is it finding some method calls (strlen and printf):
```
puts@@GLIBC_2.2.5
_edata
strlen@@GLIBC_2.2.5
printf@@GLIBC_2.2.5
__libc_start_main@@GLIBC_2.2.5
__data_start
```

It looks like an extremely easy way to get a password that is just stored in the executable as a literal. However, it seems the person who created this one was smart enough to prevent that.
