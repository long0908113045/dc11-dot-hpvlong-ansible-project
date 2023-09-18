# dc11-dot-hpvlong-ansible-project
To verify install ansible :
```bash
  ansible --version
```
To install ansible :
```bash
  sudo apt-add-repository ppa:ansible/ansible
  sudo apt update
  sudo apt install ansible -y
```
To create ssh key to ssh hosts :
```bash
  ssh-keygen -t rsa -b 4096
```
To copy ssh_pub_key to hosts :
```bash
  ssh-copy-id -i ~/.ssh/id_rsa user@host
```
To run ansible playbook with hosts :
```bash
  ansible-playbook -i hosts jenkins-config.yml
```