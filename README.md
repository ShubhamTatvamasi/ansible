# ansible

### Special Variables

https://docs.ansible.com/ansible/latest/reference_appendices/special_variables.html

test ansible connection:
```bash
ansible all -m ping
```

list all hosts:
```bash
ansible all --list-hosts
```

gather facts from servers:
```bash
ansible all -m gather_facts
ansible all -m gather_facts --limit vagrant@172.28.128.3
ansible all -m gather_facts --limit vagrant@172.28.128.6 | grep ansible_distribution
```

Install packages on server:
```bash
# update cache on servers
ansible all -m apt -a update_cache=true --become --ask-become-pass
# install apps
ansible all -m apt -a name=cowsay --become --ask-become-pass
# install latest version of the app
ansible all -m apt -a "name=cowsay state=latest" --become --ask-become-pass
# upgrade system
ansible all -m apt -a upgrade=dist --become --ask-become-pass
```
> password: `vagrant`

---

Start apache server on CentOS
```bash
sudo systemctl start httpd
```

---

generate key for ansible:
```bash
mkdir -p ~/.ssh/ansible/
ssh-keygen -t ed25519 -N '' -C "ansible" -f ~/.ssh/ansible/id_ed25519
```
