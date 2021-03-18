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

