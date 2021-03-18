# ansible

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

