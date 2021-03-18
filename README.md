# ansible

start ansible vagrant boxes:
```bash
vagrant up
```

check if servers are running:
```bash
vagrant status
```

ssh inside ansible server:
```bash
vagrant ssh ansible_server_1
```

stop vagrant servers:
```bash
vagrant halt
```

delete vagrant boxes:
```bash
vagrant destroy -f
```

get all ssh config for boxes:
```bash
vagrant ssh-config
```

ssh to server:
```bash
ssh vagrant@localhost -p $(vagrant port ansible_server_1 --guest 22)
```
> this will work if you have added your own public key to the server

