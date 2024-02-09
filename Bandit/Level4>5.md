# Bandit Level 4 → Level 5

## Level Goal

In this level, your goal is to find the password for Bandit Level 5. The password is stored in a file located in the only human-readable file in the inhere directory, which is at the home directory of the Bandit Level 4 user. Your objective is to locate this file, read its contents, and retrieve the password for the next level.

## Instructions

1. **Log into Bandit Level 4:**
   Use the password acquired from the previous level to log into Bandit Level 4. The SSH command remains unchanged:

   ```bash
   ssh bandit4@bandit.labs.overthewire.org -p 2220
   ```

2. **Navigate to the Inhere Directory:**
   Once logged in, change your current directory to the `inhere` directory using the `cd` command:

   ```bash
   cd inhere
   ```

3. **Locate the Human-Readable File:**
   Use the `file` command to identify the only human-readable file in the `inhere` directory:

   ```bash
   file ./*
   ```

   Look for the file that is identified as ASCII text. This is the human-readable file.

4. **Read the File Content:**
   Retrieve the password by reading the content of the identified human-readable file. Use the `cat` command:

   ```bash
   cat <filename>
   ```

   Replace `<filename>` with the actual name of the human-readable file.

5. **Log into Bandit Level 5:**
   Use the obtained password to log into the next level.

## Key Concepts

- **Identifying Human-Readable Files:** Learn to use the `file` command to identify the type of content within files. This is particularly useful when dealing with binary and text files.

- **Changing Directories:** Understand how to navigate through directories using the `cd` command to access specific locations in the file system.

## Tips

- **Wildcard Usage:** The `*` wildcard in the `file` command is used to match all files in the current directory.

- **Handling Spaces in Filenames:** If the filename contains spaces, enclose it in quotes or use escape characters.

## Conclusion

Completing Bandit Level 4 → Level 5 reinforces your skills in navigating directories, identifying file types, and extracting information from specific files. Understanding how to use commands like `file` and `cat` to inspect and read files is crucial in various Unix/Linux scenarios.