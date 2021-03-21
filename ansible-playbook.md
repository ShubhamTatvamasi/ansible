# ansible playbook

Install apache from ansible-playbook
```bash
ansible-playbook --ask-become-pass install_apache.yaml
```

Remove apache from ansible-playbook
```bash
ansible-playbook --ask-become-pass remove_apache.yaml
```

list all the tags on a playbook
```bash
ansible-playbook --list-tags site.yaml
```

only run tasks with `centos` tag:
```bash
ansible-playbook --tags centos --ask-become-pass site.yaml
ansible-playbook --tags "centos,db" --ask-become-pass site.yaml
```

bootstrap your servers:
```bash
ansible-playbook --ask-become-pass bootstrap.yaml
```

run playbooks without password
```bash
ansible-playbook site.yaml
```
