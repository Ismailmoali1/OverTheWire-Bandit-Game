
# OverTheWire: Bandit — Notes (Levels 1–15)

This repository contains my notes from the OverTheWire Bandit wargame.
Each level includes a brief explanation of what it teaches and the commands used to complete it


## Level 1

**Description:**  
The password for the next level is stored in a file named `readme` in the home directory.  
Retrieve this password and use it to log in to **bandit1** via SSH on port **2220**.  
For every level, use the password you discover to SSH into the next level and continue the game.

**Task:**  
List the files in the directory and read the `readme` file.

**Commands Used:**

```bash
ls
cat readme
```

Password: `ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If`

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

Password: 
`263JGJPfgU6LtdEvgfWU1XP5yac29mFx`

---
