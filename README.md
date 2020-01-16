# apache2.4_on_cent7_by_ansible
apache2.4 on cent7 by ansible

* playbookコマンド
```
ansible-playbook -i hosts webserver.yml --ask-become-pass
```

* 前提条件
```
yum install -y ansible
useradd -m ansible
passwd ansible
usermod -a -G ansible wheel
su ansible
mkdir ~/.ssh
chmod 700 ~/.ssh
cd ~/.ssh
ssh-keygen -t rsa
mv id_rsa.pub authorized_keys
chmod 600 authorized_key
```
