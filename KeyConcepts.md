# Understanding SSH (Secure Shell)

- SSH is a way to securely connect to a remote system (like GIthub).
- SSH keys help authenticate you without entering a password each time.
- Once connected via SSH, you can interact with the Github repo using git commands.

### How SSH works with Github
- You generate an SSH key on your local machine(**id_rsa**&**id_rsa.pub**)
- You add the public key(**id_rsa.pub**) to Github (under SSH keys in settings)
- Now, when you run git commands, Github uses your privacy key(id_rsa) to verify you.
- No need to enter your Github password everytime.

```
SSH is the first step to securly connect your local machine to a Github repo.
After setting it up, you can access and modify files without logging in every time. 
```
**HTTPS** - HyperText Transfer Protocol Secure

### SSH vs HTTPS
|    Feature    |       SSH       |      HTTPS        |
|---------------|-----------------|-------------------|
|    Security   | More Secure (Key-based)     | Less Secure (Password-based)|
|    Speed      | Slightly faster | Slightly slower (credentials needed) |
|    Best for   | Frequent users, automation, large teams | Occasional users, quick setup|
|   Purpose     | Secure remote access to systems & encrypted file transfers | Secure web communication over the internet
|   Use Cases   | Logging into remote servers, Git authentication, executing commands remotely| Browsing websites, API requests, Git operation|
