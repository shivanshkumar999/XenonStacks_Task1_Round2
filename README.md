# XenonStacks_Task1_Round2

Submitted by - Shivansh Kumar
With Reference to - University Recruitment Process

# internsctl - Custom Linux Command

## Introduction

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

## OPTIONS:

--help: Display help information.
--version: Display the command version.

## COMMANDS:

**cpu**: Get CPU information.
**memory**: Get memory information.
**user create <username>**: Create a new user.
**user delete <username>**: Delete a user.
**user list [--sudo-only]**: List all users or users with sudo permissions.
**file getinfo [OPTIONS] <file-name>**: Get information about a file.

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
