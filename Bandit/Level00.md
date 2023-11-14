# Bandit Level 0

## Level Goal

The primary objective of Bandit Level 0 is to introduce players to logging into a server using SSH (Secure Shell). SSH is a network protocol that provides a secure way to access a remote server. In this level, you'll connect to the OverTheWire Bandit game server using SSH.

## Details

- **Host:** bandit.labs.overthewire.org
- **Port:** 2220
- **Username:** bandit0
- **Password:** bandit0

Your task is to use these credentials to log into the server. Once you are logged in, you'll be ready to proceed to Bandit Level 1.

## Instructions

1. **Open your Terminal:** Start by opening your terminal or command line interface.

2. **Connect via SSH:**
   Use the SSH command followed by the username, host, and port number. The general syntax is `ssh [username]@[host] -p [port]`. For this level, the command will be:

   ```bash
   ssh bandit0@bandit.labs.overthewire.org -p 2220
   ```

3. **Enter the Password:** When prompted, enter the password `bandit0`. Note that while typing the password, it will not be displayed on the screen; this is a standard security feature in Unix/Linux systems.

4. **Explore the Environment:** Once logged in, feel free to explore the environment. You can try basic commands like `ls`, `pwd`, or `whoami` to get a feel for the Unix command line.

5. **Proceed to the Next Level:** After logging in, your task for this level is complete. You can now proceed to the Level 1 page for your next challenge.

## Key Concepts

- **SSH (Secure Shell):** A protocol used to securely access remote machines over a network. It encrypts all traffic to eliminate eavesdropping, connection hijacking, and other network-level attacks.

- **Terminal/Command Line Interface:** A text-based interface used to interact with your computer. Familiarity with the command line is essential in cybersecurity.

## Tips

- **SSH Client:** Ensure your computer has an SSH client installed. Most Unix/Linux systems and MacOS come with SSH pre-installed. Windows users can use clients like PuTTY or the built-in Windows Subsystem for Linux (WSL).

- **Troubleshooting:** If you cannot connect, check your internet connection and ensure you are using the correct host, port, and credentials.

- **Security Warning:** Remember that your password will not be visible as you type it. This is normal and a security feature in most terminal applications.

## Conclusion

Congratulations on completing Bandit Level 0! This level serves as your introduction to SSH and the Unix command line, both of which are fundamental skills in the world of cybersecurity. As you move to higher levels, you'll encounter more complex challenges that build upon these basics.
