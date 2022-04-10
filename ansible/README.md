#### Ansible

##### Installation
```bash
sudo apt update && sudo apt upgrade -y && sudo apt install -y python3 python3-pip git \
&& sudo update-alternatives --install /usr/bin/python python /usr/bin/python3 2 && pip3 install ansible
```

##### Check connection
```bash
ansible all -m ping
```
