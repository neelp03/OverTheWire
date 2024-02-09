# Bandit Level 2 → Level 3

## Level Goal

In this level, your objective is to find the password for Bandit Level 3. The password is stored in a file named `spaces in this filename`. The file is located in the home directory of the Bandit Level 2 user. Your task is to extract the password from this file and use it to access the next level.

## Instructions

1. **Log into Bandit Level 2:**
   Utilize the password acquired from the previous level to log into Bandit Level 2. The SSH command remains the same:

   ```bash
   ssh bandit2@bandit.labs.overthewire.org -p 2220
   ```

2. **Locate the File:**
   After successfully logging in, use the `ls` command to view the contents of the home directory:

   ```bash
   ls
   ```

   Identify a file named `spaces in this filename` among the listed files.

3. **Read the File Content:**
   Reading the file content requires handling spaces in the filename. To achieve this, you can enclose the filename in quotes or use escape characters. Two examples are provided:

   - Using quotes:
     ```bash
     cat "spaces in this filename"
     ```

   - Using escape characters:
     ```bash
     cat spaces\ in\ this\ filename
     ```

   Either of these commands will display the password for Bandit Level 3.

4. **Log into Bandit Level 3:**
   Use the obtained password to log into the next level.

## Key Concepts

- **Handling Filenames with Spaces:** This level builds on the previous one by introducing filenames with spaces. Understanding how to properly reference files with spaces is essential in Unix/Linux environments.

- **Quoting and Escape Characters:** Learn the use of quotes or escape characters to deal with filenames containing spaces. This is a common challenge in command-line operations.

## Tips

- **Explore Other Commands:** Experiment with additional commands such as `file`, `du`, and `find` on the file with spaces in the filename to gain more insights.

- **Practice Command Flexibility:** Being adaptable with quoting and escape characters will prove beneficial in various command-line scenarios.

## Conclusion

Completing Bandit Level 2 → Level 3 enhances your proficiency in handling filenames with spaces in Unix/Linux environments. The experience gained is valuable not only in overcoming specific challenges but also in preparing you for diverse scenarios involving unconventional filenames and command-line operations.