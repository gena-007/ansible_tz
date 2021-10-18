# ansible_tz
This ansible tz


this playbook:
- disable celinux on centos8 hosts
- disable firewalld on centos8 hosts
- setup and configure nginx on frontend hosts 
- setup and configure netdata on backend hosts on ports 19999


Prepare to use ansible:
 - sudo echo "$(whoami) ALL=(ALL) NOPASSWD:ALL" | sudo tee /etc/sudoers.d/$(whoami) - run on remote systems
 - sudo vi /etc/hosts and add hosts - run on central host
 - ssh-copy-id "username"@"remote_host" - copy public key on remote hosts
 
Run playbook:
ansible-playbook playbook -i hosts
