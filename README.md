## Pre Installation

- [ ] Install Ansible and Git
```bash
sudo dnf install ansible git
```

- [ ] Setup SSH Key
```
ssh-keygen -t ed25519 -C "glensutton@fastmail.com"
cat ~/.ssh/id_ed25519.pub
```

[ ] Prepare Manual Files
- Transfer .AppImage files to /home/glen/.appImage/

## Installation

- [ ] Run the playbook
```bash
ansible-pull -U git@github.com:solentenglish/ansible-fedora.git -r requirements.yml --accept-host-key --ask-become-pass
```


## Post installation
- [ ] Make refind default bootloader
```
sudo refind-mkdefault
```
- [ ] Set wallpaper
- [ ] Apply Konsave settings
```bash
konsave -a /var/tmp/settings.knsv
konsave -i settings
```



