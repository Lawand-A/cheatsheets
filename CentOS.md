Sure, here is the improved Markdown for your GitHub README:

## Connection

| Command                                     | Description                                           |
|---------------------------------------------|-------------------------------------------------------|
| `nmcli dev connect <interface_name>`         | Connect to the Internet (connect to the interface)    |
| `nmcli dev wifi connect <SSID> password <password>` | Connect to the Internet (connect to the WiFi interface)    |
| `nmcli connection show`                      | Show active connections                              |
| `nmcli connection down <connection_name>`    | Disconnect the interface                              |
| `nmcli dev disconnect <wlan_interface>`      | Disconnect WLAN connection                             |

## System

| Command                                     | Description                                           |
|---------------------------------------------|-------------------------------------------------------|
| `systemctl`                                | Show all running services                             |
| `systemctl status <service_name>`            | Show the status of a service                           |
| `journalctl -u <service_name>`              | Show log information of a service                      |
| `journalctl -fu <service_name>`             | Show log information of a service live                 |
| `journalctl -n <number_of_lines> -u <service_name>` | Show n lines of the log of a service             |
| `cat /var/log/httpd`                         | The log file for httpd                                 |

## Password Expiry

| Option                                      | Description                                           |
|---------------------------------------------|-------------------------------------------------------|
| `-M`                                        | Maximum number of days between password changes       |
| `-m`                                        | Minimum number of days between password changes       |
| `-W`                                        | Number of days of warning before the password expires |

## Hostname

| Command                                     | Description                                           |
|---------------------------------------------|-------------------------------------------------------|
| `sudo hostname <new_hostname>`               | Set temporarily the system hostname to the specified value |
| `sudo hostnamectl set-hostname <hostname>`   | Sets the system hostname to the specified value         |
| `cat /etc/hostname`                          | Show the hostname                                      |

## Groups

| Command                                     | Description                                           |
|---------------------------------------------|-------------------------------------------------------|
| `groups`                                   | Show what group you are in                             |
| `groups <username>`                         | Show what group <username> is in                       |
| `cat /etc/groups`                           | List all groups in the system                          |
| `sudo groupadd <group_name>`                | Add a new group                                       |
| `sudo groupadd -g <group_number> <group_name>` | Add a new group with a specific group number        |
| `sudo groupdel <group_name>`                | Delete a group                                        |
| `sudo usermod -aG <group_name> <user_name>` | Add a user to a group                                  |
| `sudo usermod -aG wheel <user_name>`        | Add a user to the sudo group                            |
| `sudo gpasswd -d <username> <group_name>`   | Delete a user from a group                             |

## Sudo Access

| Command                                     | Description                                           |
|---------------------------------------------|-------------------------------------------------------|
| `cat /etc/sudoer`                           | Where the sudo command is stored                       |
| `sudo -l`                                   | Show what commands the user can use as root             |
| `sudo visudo`                               | Change the sudo command                                 |
| `sudo EDITOR=nano visudo`                   | Change the sudo command using nano                     |
| `q:`                                        | To quit and force save changes in visudo               |
| `x:`                                        | To exit without saving changes in visudo               |
| `e:`                                        | To re-edit the changes in visudo                        |

## Users

| Command                                     | Description                                           |
|---------------------------------------------|-------------------------------------------------------|
| `cat /etc/passwd`                           | List of all users                                      |
| `sudo adduser <username>`                   | Add a user                                            |
| `passwd <username>`                         | Change the password for a specific user                |
| `su - <username>`                           | Change the user                                       |
| `sudo userdel <username>`                   | Delete a user                                         |
| `sudo userdel -r <username>`                | Delete a user and all their files in the home directory |


## Security and processes

| Command                                     | Description                                           |
|---------------------------------------------|-------------------------------------------------------|
| `ps aux`                                    | List all processes with details such as process ID (PID), CPU usage, memory usage, and more|
| `ps aux \| grep <process_name>`                                    | Show a process with details such as process ID (PID), CPU usage, memory usage, and more|
| `kill <PID>`                                | To Kill the process with the <PID> |
| `kill -9 <PID>`                             | Forcefully kill the process with <PID> |
| `netstat -tulpn`                           | Check network connections |
| `sudo rkhunter --check`                   | Rootkit detection to identify any hidden malicious software |
| `sudo aide --init`                | Aide is used to monitor and report changes to critical system files |
| `sudo aide --check`                | To run checks |
| `sudo iptables -L`                | Review firewall rules to make sure that only necessary ports are open |



