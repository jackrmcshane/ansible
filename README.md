# Automated Workstation Configuration and Dotfile Deployment Using Ansible

## Instructions for use

To deploy, run:
```sh
sudo apt update && sudo apt -yy upgrade
sudo apt install -yy git xclip ansible
ssh-keygen -f "/home/<username>/.ssh/id_rsa" -P "" -t rsa
cat /home/<username>/.ssh/id_rsa.pub | xclip -sel clipboard
```

Post your public key to GitHub, and finally, run:
```sh
ansible-pull -U 'https://github.com/jackrmcshane/ansible.git'
```
