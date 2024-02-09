# Bandit Level 6 → Level 7

## Level Goal

In this level, your goal is to find the password for Bandit Level 7. The password is stored somewhere on the server and has specific properties: it must be owned by user `bandit7`, owned by group `bandit6`, and have a size of 33 bytes. Your task is to locate the file meeting these criteria, read its contents, and retrieve the password for the next level.

## Instructions

1. **Log into Bandit Level 6:**
   Use the password obtained from the previous level to log into Bandit Level 6. The SSH command remains the same:

   ```bash
   ssh bandit6@bandit.labs.overthewire.org -p 2220
   ```

2. **Locate the Password File:**
   Use the `find` command along with various options to search for the password file. The file should meet the criteria of being owned by user `bandit7`, owned by group `bandit6`, and have a size of 33 bytes:

   ```bash
   find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
   ```

   This command searches for files on the entire server (`/`) that are owned by user `bandit7`, owned by group `bandit6`, and have a size of 33 bytes. The `2>/dev/null` part suppresses error messages for directories you don't have permission to access.

3. **Read the File Content:**
   Once you identify the correct file, use the `cat` command to read its content:

   ```bash
   cat <filename>
   ```

   Replace `<filename>` with the actual name of the file you found.

4. **Log into Bandit Level 7:**
   Use the obtained password to log into the next level.

## Key Concepts

- **Using `find` with Ownership and Size:** Learn how to use the `find` command to search for files based on ownership and size criteria.

- **Suppressing Error Messages:** Use `2>/dev/null` to suppress error messages when searching for files in directories you don't have permission to access.

## Tips

- **User and Group Ownership:** Understanding the concepts of user and group ownership is crucial for efficiently navigating Unix/Linux file systems.

- **Handling File Size Units:** In the `find` command, `c` denotes bytes. You can use `k` for kilobytes or `M` for megabytes.

## Conclusion

Completing Bandit Level 6 → Level 7 further hones your skills in using the `find` command to search for files based on specific ownership and size criteria. This knowledge is applicable in real-world scenarios, especially when dealing with file permissions and access control in Unix/Linux environments.