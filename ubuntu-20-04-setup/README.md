# Setup an Ubuntu 20.04 Server

The following is handled out of the box:
* User setup
* SSH hardening
* Firewall setup

It will also install the following software:
* Fail2Ban
* Git
* rclone

## Configuration

Within the provision.yml adapt the following variables: 
- username
- user_password
- public_key:

Set your correct host.


## Usage

Run the following command in your terminal:

```shell
ansible-playbook provision.yml --ask-pass
```

If you occur problems add -v to the command for verbose output. You can increase the information through -vvv or -vvvv to enable connection debugging.