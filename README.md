
# OverTheWire: Bandit — Notes (Levels 1–15)

This repository contains my notes from completing the **Bandit** wargame on OverTheWire.  
Each level includes a short explanation of the challenge, what it demonstrates, and the commands used to solve it.

---

## Level 1

**Description:**  
The password for the next level is stored in a file named `readme` in the home directory.  
After retrieving it, use the password to log in to **bandit1** via SSH on port **2220**.  
You'll repeat this process for every level: find the password, then use it to connect to the next account.

**Task:**  
List the files in the directory and read the contents of the `readme` file.

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

Password: `263JGJPfgU6LtdEvgfWU1XP5yac29mFx`

---



