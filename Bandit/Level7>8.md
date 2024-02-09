# Bandit Level 7 → Level 8

## Level Goal

In this level, your objective is to find the password for Bandit Level 8. The password is stored in the file `data.txt` next to the word "millionth." Your task is to locate this file, extract the password, and use it to access the next level.

## Instructions

1. **Log into Bandit Level 7:**
   Use the password obtained from the previous level to log into Bandit Level 7. The SSH command remains the same:

   ```bash
   ssh bandit7@bandit.labs.overthewire.org -p 2220
   ```

2. **Locate the Password File:**
   Use the `grep` command to search for the word "millionth" in the `data.txt` file:

   ```bash
   grep millionth data.txt
   ```

   This command will display the line containing the word "millionth" from the `data.txt` file.

3. **Extract the Password:**
   Extract the password from the line displayed by `grep`. You can use various text manipulation commands like `awk` or `cut` to extract the specific part containing the password.

   ```bash
   grep millionth data.txt | awk '{print $2}'
   ```

   Replace `awk '{print $2}'` with the appropriate command if the password is in a different position in the line.

4. **Log into Bandit Level 8:**
   Use the obtained password to log into the next level.

## Key Concepts

- **Searching for Specific Words:** Use the `grep` command to search for specific words within a file.

- **Text Manipulation:** Utilize commands like `awk` or `cut` to manipulate and extract specific portions of text.

## Tips

- **Understanding File Content:** Use commands like `cat` or `less` to inspect the contents of the `data.txt` file before applying `grep`.

- **Experiment with Different Commands:** Depending on the structure of the line containing the word "millionth," you may need to adjust the text manipulation command accordingly.

## Conclusion

Completing Bandit Level 7 → Level 8 reinforces your understanding of searching for specific words within files and extracting relevant information using text manipulation commands. These skills are essential for navigating and extracting valuable data from text files in Unix/Linux environments.