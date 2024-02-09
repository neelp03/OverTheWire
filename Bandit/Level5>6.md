# Bandit Level 5 → Level 6

## Level Goal

In this level, your objective is to find the password for Bandit Level 6. The password is stored in a file under the `inhere` directory and has specific properties: it must be human-readable, have a size of exactly 1033 bytes, and not be executable. Your task is to locate the file meeting these criteria, read its contents, and retrieve the password for the next level.

## Instructions

1. **Log into Bandit Level 5:**
   Use the password obtained from the previous level to log into Bandit Level 5. The SSH command remains the same:

   ```bash
   ssh bandit5@bandit.labs.overthewire.org -p 2220
   ```

2. **Navigate to the Inhere Directory:**
   Once logged in, change your current directory to the `inhere` directory using the `cd` command:

   ```bash
   cd inhere
   ```

3. **Locate the Password File:**
   Use the `find` command along with various options to search for the password file. The file should meet the criteria of being human-readable, 1033 bytes in size, and not executable:

   ```bash
   find . -type f -size 1033c ! -executable -exec file {} \; | grep ASCII
   ```

   This command searches for files under the current directory (`.`) that are 1033 bytes in size, not executable, and outputs their type using the `file` command. The `grep ASCII` filters for human-readable files.

4. **Read the File Content:**
   Once you identify the correct file, use the `cat` command to read its content:

   ```bash
   cat <filename>
   ```

   Replace `<filename>` with the actual name of the file you found.

5. **Log into Bandit Level 6:**
   Use the obtained password to log into the next level.

## Key Concepts

- **Using `find` Command:** Understand how to utilize the `find` command to search for files based on specific criteria such as size, type, and executability.

- **Filtering with `grep`:** Learn how to filter the output of commands using `grep` to narrow down results.

## Tips

- **Understanding File Size Units:** In the `find` command, `c` denotes bytes. You can use `k` for kilobytes or `M` for megabytes.

## Conclusion

Completing Bandit Level 5 → Level 6 enhances your proficiency in using the `find` command to locate files based on specific properties. This knowledge is valuable in various Unix/Linux scenarios, especially when searching for files with particular characteristics.