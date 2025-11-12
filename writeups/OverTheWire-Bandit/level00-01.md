# OverTheWire: Bandit — Level 0 → Level 1

Find the password for the next level stored in a file called `readme` in the home directory.

We start by connecting to the remote server using the provided credentials:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220

The username for this level is bandit0 and the password is also bandit0.

# Steps
    > ls (self explanatory used to list all files within directory)
    > cat readme (reads the file "readme" to find password as stated in question)

The commands outputs the following:

<img width="676" height="165" alt="image" src="https://github.com/user-attachments/assets/a680e3af-91ea-469d-9e6b-23ec4b0cbea6" />

This contains the password needed to move on to the next level.

To log in to Level 1, we use the retrieved password:

ssh bandit1@bandit.labs.overthewire.org -p 2220

That’s it — Level 0 is complete.

**[Password for Level 1: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If]**
