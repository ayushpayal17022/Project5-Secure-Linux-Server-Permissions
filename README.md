# Project 5 - Secure Linux Server Permissions

## Objective
Implement Linux user and group based access control using ownership and permissions.

## Users and Groups

Created group:

- developers

Created users:

- john
- alice
- bob

## Commands Used

```bash
sudo groupadd developers

sudo useradd -m john
sudo useradd -m alice
sudo useradd -m bob

sudo usermod -aG developers john
sudo usermod -aG developers alice

sudo mkdir /shared_data

sudo chown root:developers /shared_data

sudo chmod 770 /shared_data
