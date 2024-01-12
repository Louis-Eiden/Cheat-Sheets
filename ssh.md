# ssh Cheat Sheet

A cheat sheet for ssh commands.

#

### start ssh-agent in the background

> eval "$(ssh-agent -s)"

### show current ssh keys

> ssh-add -l

### add ssh key to ssh-agent

> ssh-add /.ssh/mykey

### Delete all keys

> ssh-add -D

### Delete a specific key

> ssh-add -d /.ssh/mykey

### Create a new ssh key

> ssh-keygen -t rsa -b 4096 -C "

#

## Generating a new key for Github and adding it to the ssh agent

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

### 1. go to repo directory

> ssh-keygen -t ed25519 -C "your_github_email@example.com"

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
