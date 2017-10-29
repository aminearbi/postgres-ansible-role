Postgres 9.5 Installation Role for Fedora / Centos 7
------------------------------

 1. install ansible on your machine `sudo yum install ansible -y`
 2. check ansible installation by passing `ansible --version` this should return your ansible version if it's installed
 3.  clone the project in your machine `git clone git@github.com:aminearbi/postgres-ansible-role.git`
 4. Edit the file called `hosts` and replace `yourserver` ip with the server you're willing to work on.
 5. On your remote server create a sudo user with and add your ssh key to its list of authorized_keys
 6. open terminal in the cloned folder and run this command `ansible-playbook playbook.yml -i hosts -u "your server user"` 
 