## Prerequisits:
- Ubuntu 20.04 Server with LAMP Stack (as described in this article: #TODO)
- Domain

## Configuration
### 1. Adapt provision.yml
1. Specify the correct hosts.
2. Specify your username.
3. Specify the path to your private key.

### 2. Set your variables
Go to ./group_vars/all and adapt the following setting to your needs:
- wp_db_name
- wp_db_password
- mysql_root_password
- server_hostname

The wp_db_user and mysql_user can be left as is or adapted.

## Usage
Run the following command in your terminal:

```shell
ansible-playbook provision.yml --ask-become-pass
```

If you occur problems add -v to the command for verbose output. You can increase the information through -vvv or -vvvv to enable connection debugging.