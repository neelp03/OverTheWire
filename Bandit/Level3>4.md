# Bandit Level 3 → Level 4

## Level Goal

In this level, your task is to discover the password for Bandit Level 4. The password is stored in a hidden file named `.hidden` within the home directory of the Bandit Level 3 user. Your objective is to retrieve the password from this hidden file and use it to access the next level.

## Instructions

1. **Log into Bandit Level 3:**
   Use the password obtained from the previous level to log into Bandit Level 3. The SSH command remains consistent:

   ```bash
   ssh bandit3@bandit.labs.overthewire.org -p 2220
   ```

2. **Locate the Hidden File:**
   After successfully logging in, use the `ls` command with the `-a` option to display hidden files in the home directory:

   ```bash
   ls -a
   ```

   Identify a hidden file named `.hidden` among the listed files.

3. **Read the File Content:**
   Retrieve the password by reading the content of the `.hidden` file. Utilize the `cat` command:

   ```bash
   cat .hidden
   ```

   This command will display the password for Bandit Level 4.

4. **Log into Bandit Level 4:**
   Use the acquired password to log into the next level.

## Key Concepts

- **Hidden Files:** Learn how to reveal and interact with hidden files in Unix/Linux by using the `-a` option with the `ls` command.

- **Reading Hidden File Content:** Familiarize yourself with reading the content of hidden files using standard commands like `cat`.

## Tips

- **Understanding Hidden Files:** The dot (`.`) prefix in Unix/Linux signifies hidden files. Always check for hidden files when searching for specific information.

- **Experiment with Permissions:** In later levels, understanding file permissions becomes crucial. Take note of the permissions of the hidden file.

## Conclusion

Completing Bandit Level 3 → Level 4 enhances your ability to work with hidden files and reinforces fundamental command-line skills. Understanding how to uncover and interact with hidden files is essential for navigating Unix/Linux systems effectively.