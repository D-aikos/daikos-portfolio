# OverTheWire: Bandit — Level 2 → Level 3

Search for a file named `spaces in this filename` and read its contents to find the password.

We start by connecting to the remote server using the provided credentials:

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
The password for this level is [263JGJPfgU6LtdEvgfWU1XP5yac29mFx]

# Steps
    > ls -alps (self explanatory used to list all files within directory with some important metadate)
    > cat ./"--spaces in this filename--" (if there spaces in the file name along with -- use both ./ and "" to send file name to command)

The commands outputs the following:
<img width="639" height="164" alt="image" src="https://github.com/user-attachments/assets/6a181141-84f4-417b-942a-af086c2841eb" />

This contains the password needed to move on to the next level.
To log in to Level 3, we use the retrieved password:
ssh bandit3@bandit.labs.overthewire.org -p 2220

That’s it — Level 2 is complete.

**[Password for Level 3: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx]**
