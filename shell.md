# Shell Cheat Sheet

---
## **UNDER CONSTRUCTION**
---

reset location hash to #shell

```Shell
hash -r
```

## Shell Scripting

### Variables

```Shell
# Declaring variables
name="John Doe"
age=30
```

```Shell
# Variable naming conventions
# - Variable names must begin with a letter or underscore
# - Variable names can only contain letters, numbers, and underscores
# - Variable names are case-sensitive
```

```Shell
# Using variables
echo "My name is $name and I am $age years old."
```

```Shell
# Using command substitution
echo "Today is $(date +%A)."
```

```Shell
# Using arithmetic expansion
echo "The result of 5 + 5 is $((5 + 5))."
```

```Shell
# Using the read command
read -p "Enter your name: " name
echo "Hello $name, nice to meet you!"
```

```Shell
# Using the read command with a timeout
read -t 5 -p "Enter your name: " name
echo "Hello $name, nice to meet you!"
```

```Shell
# Using the read command with a default value
read -p "Enter your name [John]: " name
name=${name:-John}
echo "Hello $name, nice to meet you!"
```

```Shell
# Using the read command with a prompt loop
while read -p "Enter your name: " name && [[ -z $name ]]; do
  echo "Please enter your name."
done
echo "Hello $name, nice to meet you!"
```

```Shell
# Using the read command with a password prompt
read -sp "Enter your password: " password
echo "Your password is $password."
```

```Shell
# Using the read command with a password prompt and a timeout
read -t 5 -sp "Enter your password: " password
echo "Your password is $password."
```

```Shell
# Using the read command with a password prompt and a default value
read -sp "Enter your password [password]: " password
password=${password:-password}
echo "Your password is $password."
```

```Shell
# Using the read command with a password prompt and a prompt loop
while read -sp "Enter your password: " password && [[ -z $password ]]; do
  echo "Please enter your password."
done
echo "Your password is $password."
```
