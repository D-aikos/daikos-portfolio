# OverTheWire: Bandit — Level 1 → Level 2

Read a file with restricted permissions to retrieve the next level password.

We start by connecting to the remote server using the provided credentials:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
The password for this level is [ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If]

# Steps
    > ls -alps (self explanatory used to list all files within directory with some important metadate)
    > cat ./- (reads the file "-" to find password as stated in question. To read dashed files use ./ to seperate name from command)

The commands outputs the following:
<img width="520" height="163" alt="image" src="https://github.com/user-attachments/assets/d8639cc6-27ea-4262-a656-296229d2cac9" />

This contains the password needed to move on to the next level.
To log in to Level 2, we use the retrieved password:
ssh bandit2@bandit.labs.overthewire.org -p 2220

That’s it — Level 1 is complete.

**[Password for Level 2: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx]**
