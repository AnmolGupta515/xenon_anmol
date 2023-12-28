internsctl - Custom Linux Command for Interns
Version: v0.1.0

Overview
internsctl is a custom Linux command designed for interns to perform various system-related tasks, including user management, CPU information retrieval, memory information retrieval, and file information retrieval.
Usage
bash
Copy code
./internsctl [command] [options]
Commands
User Management
Create User
bash
Copy code
./internsctl user create <username>
Create a new user with the specified username.

List Users
bash
Copy code
./internsctl user list [--sudo-only]
List all users or only users with sudo privileges.

System Information
CPU Information
bash
Copy code
./internsctl cpu getinfo
Display CPU information similar to the lscpu command.

Memory Information
bash
Copy code
./internsctl memory getinfo
Display memory information similar to the free command.

File Information
bash
Copy code
./internsctl file getinfo [options] <file-name>
Display information about the specified file.

Options:
--size, -s: Print file size.
--permissions, -p: Print file permissions.
--owner, -o: Print file owner.
--last-modified, -m: Print last modified time.
--help: Display help message.
Examples
Create a user:

bash
Copy code
./internsctl user create john_doe
List all users:

bash
Copy code
./internsctl user list
Get CPU information:

bash
Copy code
./internsctl cpu getinfo
Get memory information:

bash
Copy code
./internsctl memory getinfo
Get file information:

bash
Copy code
./internsctl file getinfo --size --permissions myfile.txt
Help
bash
Copy code
./internsctl --help
Display the overall help message.

