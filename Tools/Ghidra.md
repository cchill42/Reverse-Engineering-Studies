## Table of Contents
- [Overview](#Overview)
- [Usage](#Usage)

## Overview
This is the second tool for reverse engineering I ever used, and it is a big step up from strings. However, there is so much functionality built into this tool. It is a disassembler, decompiler, and more built into one tool. I have found it very good to use, but it is very complex when I am first starting to use it.

## Usage

### 2/26/2026
I downloaded a simple CrackMe to test out Ghidra. Here is the code browser after analysis
<img width="1643" height="889" alt="image" src="https://github.com/user-attachments/assets/4ac8ad39-2627-4d23-807a-60d3fcd947b0" />

What I find really cool is how Ghidra takes the assembly instructions and turns them into C. As I have not learned much about assembly yet, it makes it much easier for me to understand what is going on. However, it seems it wasn't able to completely decompile it, as there are still some weird things in the C.

Ghidra lets me change certain aspects of the code and insert comments, so I can make it a lot more readable.
