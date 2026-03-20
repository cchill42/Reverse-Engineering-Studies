## Target: easy-reverse
Author: cbm-hackers

Date: 03-20-2026

Tools Used: Ghidra

Difficulty: Easy

### Goal: Find the correct password

### Approach:

I first loaded it up into Ghidra and found the main method.

<img width="1643" height="889" alt="Screenshot 2026-03-18 095202" src="https://github.com/user-attachments/assets/02d3415c-94bc-4db2-9cb7-f2d75c7e39bf" />

Then, I edited the pseudo-c code to make it more readable for me. 

<img width="1634" height="893" alt="image" src="https://github.com/user-attachments/assets/18d49118-3fb9-4f10-803d-6caaf7e0b61f" />

From this simplification, I found out the password's parameters. First, it checked if only one argument was entered. Then, it checks if the size of the string is 10.
Lastly, it checks if the character at position 4 is an '@' character. If it is, then the password is accepted.

So, I can put in a password using this format: **XXXX@XXXXX**

<img width="425" height="101" alt="image" src="https://github.com/user-attachments/assets/2e939100-fd46-4252-9b2d-4b719ff5abf8" />

And here it is solved.

### Key Findings:

The checks the program was performing on the password were pretty easy to decipher. There was no encryption involved.

### Takeaways:

This taught me a good deal about navigating Ghidra and some of the tools it provides. This was a great stepping stone into more challenging things.
