# OverTheWire: Bandit — Level 3 → Level 4

Locate a hidden file in the `inhere` directory and retrieve the password inside it.

We start by connecting to the remote server using the provided credentials:

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
The password for this level is [263JGJPfgU6LtdEvgfWU1XP5yac29mFx]

# Steps
    > ls -alps (self explanatory used to list all files within directory with some important metadata)
    > cd inhere (change the directory to inhere)
    > ls -alps (self explanatory used to list all files within directory with some important metadata)
    > cat ./"...Hiding-From-You" (if there spaces in the file name along with -- use both ./ and "" to send file name to command)

The commands outputs the following:
<img width="550" height="263" alt="image" src="https://github.com/user-attachments/assets/7c935b43-2afd-44f6-b361-1a6dce7c2ffb" />

This contains the password needed to move on to the next level.
To log in to Level 4, we use the retrieved password:
ssh bandit4@bandit.labs.overthewire.org -p 2220

That’s it — Level 3 is complete.

**[Password for Level 4: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ]**
