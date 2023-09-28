# SSH - Secure Shell Protocol

### What is SSH

- SSH, which stands for Secure Shell, is a widely-used protocol for securely accessing remote servers and devices over a network. It provides a secure way to authenticate, encrypt data, and manage remote systems.

### What is SSH used for?

- **Remote Server Administration** - Administer servers and execute commands remotely.
- **File Transfer** - Securely transfer files between your local and remote systems (e.g., using SCP or SFTP).
- **Tunneling** - Create secure tunnels for forwarding network traffic, like port forwarding.
- **Git/GitHub Access** - Authenticate and interact with remote Git repositories.
- **Database Access** - Securely access and manage databases on remote servers.

### How does SSH work?

- SSH works by using a pair of keys: a private key on your local device and a public key on the remote server. These keys enable secure authentication and data encryption for remote access and management of servers and devices.

### What are Private and Public keys?

- **Private Keys** - private and secret, only known to the user, is encrypted and stored safely
- **Public Keys** - Shared freely with any SSH server for any user to use as they wish.

### Why use SSH?

- Other than providing strong encryption, SSH is used to manage systems and applications remotely, allowing the user to access another system in the network and interacte with it.

### How does it increase security?

- SSH provides **encryption** on all data transfer, making it a secure way to transfer data, as well it provides secure access when logging into remote systems.

### How can you create a SSH key pair?

- On the terminal you can generate a SSH key pair by using the command ```ssh-keygen```


