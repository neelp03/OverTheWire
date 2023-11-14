# Bandit Level 0 → Level 1

## Level Goal

In this level, your task is to find the password for Bandit Level 1. The password is stored in a file named `readme` located in the home directory of the Bandit Level 0 user. Once you find this password, you'll use it to log into Bandit Level 1 using SSH.

## Instructions

1. **Log into Bandit Level 0:** 
   If you're not already connected, log into Bandit Level 0 using the credentials provided in the previous level (Username: `bandit0`, Password: `bandit0`). Use the SSH command:

   ```bash
   ssh bandit0@bandit.labs.overthewire.org -p 2220
   ```

2. **Locate the `readme` File:**
   Once logged in, you're in the home directory by default. Use the `ls` command to list the contents of the directory:

   ```bash
   ls
   ```

   You should see the `readme` file listed.

3. **Read the File Content:**
   Use the `cat` command to display the contents of the `readme` file, which contains the password for the next level:

   ```bash
   cat readme
   ```

   The output will be the password for Bandit Level 1.

4. **Log into Bandit Level 1:**
   Now that you have the password, you can log out from Bandit Level 0 and log into Bandit Level 1 using the new password.

## Key Concepts

- **Navigating the File System:** Understanding how to move around and inspect the file system is crucial. Commands like `ls` and `cd` are fundamental for this.
  
- **Viewing File Contents:** The `cat` command is a quick way to display the contents of a file. It's one of several commands you can use to read files in Unix/Linux.

- **File Manipulation:** Besides `cat`, familiarize yourself with commands like `file`, `du`, and `find` for handling and searching files.

## Tips

- **Exploring Further:** Feel free to experiment with other commands mentioned like `file`, `du`, and `find` to get more comfortable with them.

- **Secure Practices:** Always remember to log out from the server when you're done with a level to maintain good security practices.

## Conclusion

Completing Bandit Level 0 → Level 1 introduces you to basic file navigation and content viewing in the Unix command line, skills that are foundational in cybersecurity and system administration. Keep these concepts in mind as you advance to the next level.
