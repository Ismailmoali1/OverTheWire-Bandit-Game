
# OverTheWire: Bandit - My Notes & Walkthrough

This repository contains my personal notes from working through the **Bandit** wargame on [OverTheWire](https://overthewire.org/wargames/bandit/).

I use this repo to:
- Document how I solved each level
- Keep track of useful commands and concepts
- Build a reference I can revisit later

> ⚠️ **Spoiler warning:**  
> These notes may contain full solutions, including commands and passwords.  
> If you're playing Bandit for the first time, try each level yourself before reading further.

---

## How to Connect to Bandit

Bandit runs on port `2220` over SSH.

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

bandit0, bandit1, bandit2, ...

---

## Level 1

**Description:**  
The password for the next level is stored in a file named `readme` in the home directory.  
After retrieving it, I used the password to log in to **bandit1** via SSH on port **2220**.  
I follow this process for every level: find the password, then use it to connect to the next account.

**Task:**  
List the files in the directory and read the contents of the `readme` file.

**Commands Used:**

```bash
ls
cat readme
```

Password: `ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If`

**What I learned:**  
How to look inside a directory with `ls` and read a file using `cat`.  
This level helped me get comfortable finding and viewing basic files in Linux.

---

## Level 2

**Description:**  
The password for the next level is stored in a file called `-` located in the home directory.

**Task:**  
The file is named `-`, so it must be accessed using a relative path.

**Commands Used:**

```bash
./-
```

Password: `263JGJPfgU6LtdEvgfWU1XP5yac29mFx`

**What I learned:**  
How to open a file with a tricky name, like `-`.  
I learned that using a path like `./-` tells the system it's a file, not an option.

---

## Level 3

**Description:**  
The password for the next level is stored in a file called `spaces in this filename` located in the home directory.

**Task:**  
The filename contains spaces, so it must be wrapped in quotes when accessed.

**Commands Used:**

```bash
cat "spaces in this filename"
```

Password: `MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx`

**What I learned:**  
How to open a file that has spaces in its name.  
Putting the filename in quotes makes the command treat it as one single name.

---

## Level 4

**Description:**  
The password for the next level is stored in a hidden file inside the `inhere` directory.

**Task:**  
List all files (including hidden ones) and read the hidden file.

**Commands Used:**

```bash
ls -al
cat ...Hidding-From-You
```

Password: `2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ`

**What I learned:**  
How to find hidden files using `ls -a`.  
Hidden files start with a dot (`.`), so you need this command to see and open them.

---
