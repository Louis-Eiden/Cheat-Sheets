# ssh Cheat Sheet

---
## **UNDER CONSTRUCTION**
---

A cheat sheet for ssh commands.

[variable] = placeholder for a variable

#

```bash
eval "$(ssh-agent -s)" # start the ssh-agent in the background
ssh-add ~/.ssh/[private_key] # add ssh key to ssh-agent
ssh-add -l # show current ssh keys
ssh-add -D # delete all keys
ssh-add -d ~/.ssh/[private_key] # delete a specific key
ssh-keygen -t rsa -b 4096 -C # create a new ssh key using 4096 bit rsa encryption
ssh-keygen -p # change passphrase of an existing ssh key
ssh-keygen -y -f ~/.ssh/[private_key] > ~/.ssh/[public_key] # generate public key from private key
ssh-keygen -l -f ~/.ssh/[public_key] # show fingerprint of public key
```

#

## Generating a new key for Github and adding it to the ssh agent

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

### 1. go to repo directory

ssh-keygen -t ed25519 -C {your_github_email@example.com}

### 2. Enter a file in which to save the key (press enter to use default)

### 3. Enter passphrase (press enter to skip passphrase)

### 4. Add your SSH public key to your GitHub account:

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account

#

## Automatically add ssh key to ssh-agent on startup

### create .bash_profile file to automatically add ssh key to ssh-agent

> touch ~/.bash_profile

### add the following to the .bash_profile file

```bash
# Start the SSH agent if it's not running
if [ ! -S "$SSH_AUTH_SOCK" ]; then
    eval $(ssh-agent)
fi

# Check if the SSH key is already added
if ! ssh-add -l | grep -q "path_to_private-key"; then
    # Add the SSH key to the agent
	ssh-add path_to_private-key
fi
```

### check ssh connection to github

```bash
ssh -T git@github.com
```
