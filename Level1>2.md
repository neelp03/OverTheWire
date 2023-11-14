# Bandit Level 1 → Level 2

## Level Goal

In this level, you are tasked with finding the password for Bandit Level 2. The password is stored in a uniquely named file called `-` (just a hyphen), which is located in the home directory of the Bandit Level 1 user. Your goal is to retrieve the contents of this file to obtain the password for the next level.

## Instructions

1. **Log into Bandit Level 1:** 
   Use the password obtained from the previous level to log into Bandit Level 1. The SSH command will be:

   ```bash
   ssh bandit1@bandit.labs.overthewire.org -p 2220
   ```

2. **Locate the File:**
   Once logged in, use the `ls` command to list the files in the home directory:

   ```bash
   ls
   ```

   You'll notice a file named `-` listed among the files.

3. **Reading the File Content:**
   Normally, `cat filename` is used to display file contents. However, using `cat -` will not work as expected because the shell interprets `-` as a placeholder for standard input. To read the file, you need to help `cat` understand that `-` is a filename. There are a couple of ways to do this:

   - Using `./` (current directory) with the filename:
     ```bash
     cat ./-
     ```
   - Or using `cat` with `--` which tells `cat` that what follows is a filename:
     ```bash
     cat -- -
     ```

   Either of these commands will display the password for Bandit Level 2.

4. **Log into Bandit Level 2:**
   Use the retrieved password to log into the next level.

## Key Concepts

- **Handling Unusual Filenames:** This level teaches you how to deal with files that have non-standard or tricky names. Understanding how to specify file paths correctly is important in Unix/Linux environments.

- **Command-Line Arguments and Options:** Understanding how command-line arguments and options work is crucial. The `--` is a common way to signify the end of command options in Unix/Linux commands.

## Tips

- **Experiment with Other Commands:** Feel free to try out other mentioned commands like `file`, `du`, and `find` on the `-` file to see what information they return.

- **Standard Input and Output:** This level provides insight into how Unix/Linux interprets standard input and output, represented by `-`.

## Conclusion

Completing Bandit Level 1 → Level 2 introduces you to the concept of handling files with unusual names in the Unix/Linux command line. This knowledge is not only useful in scripting and system administration but also in understanding more complex command-line operations in future challenges.