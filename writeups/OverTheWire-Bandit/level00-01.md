# OverTheWire: Bandit — Level 0 → Level 1

**Author:** Dheemanth M Rao (D-aikos)

The goal of this level is to find the password for the next level. The password is stored in a file called `readme` located in the home directory. To retrieve it, we’ll connect to the Bandit server using SSH and explore the directory.

We start by connecting to the remote server using the provided credentials:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220

The username for this level is bandit0 and the password is also bandit0. Once logged in, we can list the files in the home directory to see what’s available:

ls

This shows a file named readme. To view its contents, we use the cat command, which prints the content of the file to the terminal:

cat readme

The command outputs the following password:

boJ9jbbUNNfktd78OOpsqOltutMc3MY1

This is the password needed to move on to the next level.

To log in to Level 1, we use the retrieved password:

ssh bandit1@bandit.labs.overthewire.org -p 2220

That’s it — Level 0 is complete.

Notes:
This level introduces basic SSH usage and simple Linux commands.
We used:

    ssh to connect to the remote server

    ls to list files in the current directory

    cat to read the contents of a file

Password for Level 1: boJ9jbbUNNfktd78OOpsqOltutMc3MY1
