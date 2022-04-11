#### User
##### Create user
Create new user
```bash
sudo useradd username
```

Add password for user
```bash
sudo passwd username
```

Use the -m (--create-home) option to create the user home directory as /home/username
```bash
sudo useradd -m username
```

##### Add sudo for user
```bash
usermod -aG sudo username
```

##### Change user
```bash
su - username
```

##### Change password
```bash
passwd
```
