## com-bootstrap
Ansible script to bootstrap client servers with commercial team users.

## Usage
Create a file called hosts with the ip addresses of the servers. For instance if there were two IP addresses, 192.168.1.1 and 192.168.1.2, it'd be defined as follows in the hosts file.

    192.168.1.1
    192.168.1.2

Now run the ansible playbook against this host file

    ansible-playbook -i hosts main.yml

You may want to use the following paramters to ansible
* `-u` to provide the user for SSH.
* `-s` to run commands as sudo.
* `-k` to ask for SSH password.
* `-K` to ask for sudo password.
