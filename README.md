# XenonStacks_Task1_Round2

Submitted by - Shivansh Kumar
With Reference to - University Recruitment Process

# internsctl - Custom Linux Command

## Introduction+

`internsctl` is a custom Linux command designed for internship operations. It provides a set of functionalities related to CPU information, memory information, user management, and file operations.

## Features

- Get detailed CPU information.
- Retrieve memory usage details.
- Manage user operations like creating and listing users.
- Obtain information about files, including size, permissions, owner, and last modification time.

## Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/your-username/internsctl.git
```

Navigate to the project directory:

```bash
cd internsctl
```
Make the script executable:
```bash
chmod +x internsctl
```
Usage

```bash
./internsctl [OPTIONS] COMMAND [ARGS]
```

## Creation of MAN file

Step 1:
```bash
nano internsctl.1
```

Step 2:
Write your information into the manual file

Step 3:
```bash
sudo mkdir -p /usr/share/man/man1
sudo mv internsctl.1 /usr/share/man/man1/
sudo mandb
```

Step 4:
```bash
man internsctl
```

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/76eae209-2f11-42fa-9b86-c554852f3049)

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/f65ae513-182e-41b4-a313-661e62b37dc5)

## OPTIONS:

<p>--help: Display help information.</p>
<p>--version: Display the command version.</p>

## COMMANDS:

**cpu**: Get CPU information.
**memory**: Get memory information.
**user create <username>**: Create a new user.
**user list [--sudo-only]**: List all users or users with sudo permissions.
**file getinfo [OPTIONS] <file-name>**: Get information about a file. like permissions, owner, filename, size, lastmodified

Options

For CPU, memory, and file commands, various options are available. See specific command sections for details.

Examples
Get CPU information:
```bash
./internsctl cpu
```
Create a new user:
```bash
./internsctl user create john_doe
```
Get information about a file, including size and permissions:
```bash
./internsctl file getinfo --size --permissions /path/to/file.txt
```

# > Section A
The working of 
```bash
man intersectl
```

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/76eae209-2f11-42fa-9b86-c554852f3049)

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/f65ae513-182e-41b4-a313-661e62b37dc5)

The working of 
```bash
internsctl --help
```
```bash
internsctl --version
```
![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/dd8b1393-68f3-405f-8019-4d61db71d6c2)


# > Section B 

## Part 1 - Easy

The working of 
```bash
internsctl cpu getinfo
```
![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/670e696e-6342-465b-aa45-fe1327a656b7)

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/d355143c-55d5-4034-9c85-05551ca0b981)


The working of 
```bash
internsctl memory getinfo
```

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/dd7f8f75-e5f8-476b-aad7-c90f71762621)


## Part 2 - Intermediate

```bash
internsctl user create 
```
![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/1b3fd3ad-49cf-4339-8293-7e4f963aaf7f)

```bash
internsctl user list
```
![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/1115d53f-4bbc-4946-9ce5-16212fc1f30e)

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/d13f8fd2-cf1f-43eb-a622-eaa99983af09)

```bash
internsctl user list --sudo-only
```
![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/d02a785a-7d6f-4405-b51e-321401976b6b)

## Part 3 - Advanced Level

Advanced Level

```bash
internsctl file getinfo
```

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/752d267e-dff9-492d-ab8f-6ddc212f38c1)

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/713f2efa-09d8-4c10-8716-74091899607a)


```bash
internsctl file getinfo --size  / internsctl file getinfo -s
```
```bash
internsctl file getinfo --permissions / internsctl file getinfo -p
```
```bash
internsctl file getinfo --owner  / internsctl file getinfo -o
```
```bash
internsctl file getinfo --last-modified  / internsctl file getinfo -m
```

![image](https://github.com/shivanshkumar999/XenonStacks_Task1_Round2/assets/67266253/c38c78fc-f118-4631-b3d5-5e92d1100235)

